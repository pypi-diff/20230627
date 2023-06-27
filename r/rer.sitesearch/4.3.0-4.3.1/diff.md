# Comparing `tmp/rer.sitesearch-4.3.0.tar.gz` & `tmp/rer.sitesearch-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.sitesearch-4.3.0.tar", last modified: Thu Mar 30 12:12:35 2023, max compression
+gzip compressed data, was "rer.sitesearch-4.3.1.tar", last modified: Tue Jun 27 12:29:55 2023, max compression
```

## Comparing `rer.sitesearch-4.3.0.tar` & `rer.sitesearch-4.3.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.462821 rer.sitesearch-4.3.0/
--rw-r--r--   0 cekk       (501) staff       (20)      397 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/.eslintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      295 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/.prettierrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      131 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/.stylelintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)     5997 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/CHANGELOG.rst
--rw-r--r--   0 cekk       (501) staff       (20)      320 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    15841 2023-03-30 12:12:35.463092 rer.sitesearch-4.3.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     4648 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.427714 rer.sitesearch-4.3.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     1459 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/docs/INSTALL.txt
--rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/docs/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      751 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/docs/LICENSE.txt
--rw-r--r--   0 cekk       (501) staff       (20)    48211 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/docs/SiteSearch_Configurazione.JPG
--rw-r--r--   0 cekk       (501) staff       (20)    81932 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/docs/SiteSearch_Risultati-ricerca.JPG
--rw-r--r--   0 cekk       (501) staff       (20)    32560 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/docs/rer-logo.png
--rw-r--r--   0 cekk       (501) staff       (20)     3194 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/package.json
--rw-r--r--   0 cekk       (501) staff       (20)      256 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/postcss.config.js
--rw-r--r--   0 cekk       (501) staff       (20)       50 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      346 2023-03-30 12:12:35.463734 rer.sitesearch-4.3.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2193 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.412407 rer.sitesearch-4.3.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.428104 rer.sitesearch-4.3.0/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)      245 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.432982 rer.sitesearch-4.3.0/src/rer/sitesearch/
--rw-r--r--   0 cekk       (501) staff       (20)      108 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.434189 rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      345 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1050 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/custom_filters.py
--rw-r--r--   0 cekk       (501) staff       (20)      845 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/permission_checker.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.435974 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2244 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1699 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1301 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/i18n.py
--rw-r--r--   0 cekk       (501) staff       (20)      202 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/interfaces.py
--rw-r--r--   0 cekk       (501) staff       (20)     1499 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/search.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.415536 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.413331 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.438521 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/
--rw-r--r--   0 cekk       (501) staff       (20)    16174 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.css
--rw-r--r--   0 cekk       (501) staff       (20)    16374 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.css.map
--rw-r--r--   0 cekk       (501) staff       (20)   689622 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.js
--rw-r--r--   0 cekk       (501) staff       (20)     1664 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.438849 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.439152 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/GroupsFilter/
--rw-r--r--   0 cekk       (501) staff       (20)     1784 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/GroupsFilter/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.440321 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/
--rw-r--r--   0 cekk       (501) staff       (20)     1403 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/boolean.js
--rw-r--r--   0 cekk       (501) staff       (20)     6227 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/date.js
--rw-r--r--   0 cekk       (501) staff       (20)     2137 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/index.js
--rw-r--r--   0 cekk       (501) staff       (20)     1570 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/select.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.440607 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/LocationFilter/
--rw-r--r--   0 cekk       (501) staff       (20)     3402 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/LocationFilter/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.440891 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     7281 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.441178 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchFilters/
--rw-r--r--   0 cekk       (501) staff       (20)     3263 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchFilters/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.442087 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.442997 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/
--rw-r--r--   0 cekk       (501) staff       (20)     3647 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/Bando.js
--rw-r--r--   0 cekk       (501) staff       (20)     1440 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/DateAndPosition.js
--rw-r--r--   0 cekk       (501) staff       (20)     7462 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/ResultItem.js
--rw-r--r--   0 cekk       (501) staff       (20)     3160 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/header.js
--rw-r--r--   0 cekk       (501) staff       (20)     2531 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/index.js
--rw-r--r--   0 cekk       (501) staff       (20)     1726 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/pagination.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.443290 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchableTextFilter/
--rw-r--r--   0 cekk       (501) staff       (20)     2703 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchableTextFilter/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.443889 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SpecificFilters/
--rw-r--r--   0 cekk       (501) staff       (20)     7415 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SpecificFilters/SpecificFilter.js
--rw-r--r--   0 cekk       (501) staff       (20)     2177 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SpecificFilters/index.js
--rw-r--r--   0 cekk       (501) staff       (20)      529 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.445634 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/
--rw-r--r--   0 cekk       (501) staff       (20)     1398 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/apiFetch.js
--rw-r--r--   0 cekk       (501) staff       (20)      690 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/i18n.js
--rw-r--r--   0 cekk       (501) staff       (20)      660 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/icons.js
--rw-r--r--   0 cekk       (501) staff       (20)      375 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/searchContext.js
--rw-r--r--   0 cekk       (501) staff       (20)     3249 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/types.js
--rw-r--r--   0 cekk       (501) staff       (20)      933 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/vocabulary.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.446210 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.446519 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/Pagination/
--rw-r--r--   0 cekk       (501) staff       (20)      217 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/Pagination/pagination.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.446815 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchFilters/
--rw-r--r--   0 cekk       (501) staff       (20)     5251 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchFilters/filters.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.447695 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchResults/
--rw-r--r--   0 cekk       (501) staff       (20)      539 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchResults/header.less
--rw-r--r--   0 cekk       (501) staff       (20)      114 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchResults/loading.less
--rw-r--r--   0 cekk       (501) staff       (20)     3059 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchResults/result_item.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.447983 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SpecificFilters/
--rw-r--r--   0 cekk       (501) staff       (20)     1212 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SpecificFilters/specific_filters.less
--rw-r--r--   0 cekk       (501) staff       (20)      304 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/generic.less
--rw-r--r--   0 cekk       (501) staff       (20)      884 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/index.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.448704 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)     1716 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/templates/search.pt
--rw-r--r--   0 cekk       (501) staff       (20)     1722 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/browser/templates/search_local.pt
--rw-r--r--   0 cekk       (501) staff       (20)     2110 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.450384 rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/
--rw-r--r--   0 cekk       (501) staff       (20)      549 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      267 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/additional_templates.py
--rw-r--r--   0 cekk       (501) staff       (20)      346 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/custom_filters.py
--rw-r--r--   0 cekk       (501) staff       (20)      282 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/layer.py
--rw-r--r--   0 cekk       (501) staff       (20)     4881 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/settings.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.451850 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.417056 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.452789 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     4576 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.mo
--rw-r--r--   0 cekk       (501) staff       (20)     8390 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.417329 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.453429 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     5079 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.mo
--rw-r--r--   0 cekk       (501) staff       (20)     8806 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.po
--rw-r--r--   0 cekk       (501) staff       (20)     1460 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)     6682 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/rer.sitesearch.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1777 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      498 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/locales/update.sh
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.417933 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.455239 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      142 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      507 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      240 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)       98 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      250 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/rolemap.xml
--rw-r--r--   0 cekk       (501) staff       (20)       50 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/default/sitesearch_various.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.455825 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/to_4000/
--rw-r--r--   0 cekk       (501) staff       (20)      274 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/to_4000/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)     1399 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/to_4000/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.457328 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      155 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      185 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      278 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/uninstall/cssregistry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      113 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      364 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/uninstall/skins.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.458117 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      233 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.459359 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     4985 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/catalog.py
--rw-r--r--   0 cekk       (501) staff       (20)      283 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      977 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/summary.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.459879 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      197 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.460673 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      587 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     7919 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search/get.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.461570 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search_filters/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search_filters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      429 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search_filters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      519 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search_filters/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     2753 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/utils.py
--rw-r--r--   0 cekk       (501) staff       (20)      421 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2226 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.462405 rer.sitesearch-4.3.0/src/rer/sitesearch/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1951 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/tests/disabled_test_search_filters_endpoint.py
--rw-r--r--   0 cekk       (501) staff       (20)     2297 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)      430 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)      686 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/upgrades.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      461 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/utils.py
--rw-r--r--   0 cekk       (501) staff       (20)     3246 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/src/rer/sitesearch/vocabularies.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-30 12:12:35.430515 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    15841 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     5956 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      139 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      218 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2023-03-30 12:12:35.000000 rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)     2780 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/webpack.config.js
--rw-r--r--   0 cekk       (501) staff       (20)   473978 2023-03-30 12:12:34.000000 rer.sitesearch-4.3.0/yarn.lock
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.649117 rer.sitesearch-4.3.1/
+-rw-r--r--   0 cekk       (501) staff       (20)      397 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/.eslintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      295 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/.prettierrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      131 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/.stylelintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)     6091 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/CHANGELOG.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      320 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    15968 2023-06-27 12:29:55.649340 rer.sitesearch-4.3.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     4648 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.618933 rer.sitesearch-4.3.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     1459 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/docs/INSTALL.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/docs/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      751 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/docs/LICENSE.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    48211 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/docs/SiteSearch_Configurazione.JPG
+-rw-r--r--   0 cekk       (501) staff       (20)    81932 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/docs/SiteSearch_Risultati-ricerca.JPG
+-rw-r--r--   0 cekk       (501) staff       (20)    32560 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/docs/rer-logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     3194 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)      256 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/postcss.config.js
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      346 2023-06-27 12:29:55.649848 rer.sitesearch-4.3.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2164 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.606760 rer.sitesearch-4.3.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.619214 rer.sitesearch-4.3.1/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)      245 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.623266 rer.sitesearch-4.3.1/src/rer/sitesearch/
+-rw-r--r--   0 cekk       (501) staff       (20)      108 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.624288 rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      345 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1050 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/custom_filters.py
+-rw-r--r--   0 cekk       (501) staff       (20)      845 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/permission_checker.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.625809 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2244 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1699 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1301 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/i18n.py
+-rw-r--r--   0 cekk       (501) staff       (20)      202 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/interfaces.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1499 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/search.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.609385 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.607522 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.628115 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/
+-rw-r--r--   0 cekk       (501) staff       (20)    16174 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.css
+-rw-r--r--   0 cekk       (501) staff       (20)    16374 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)   689622 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1664 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.628400 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.628665 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/GroupsFilter/
+-rw-r--r--   0 cekk       (501) staff       (20)     1784 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/GroupsFilter/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.629837 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/
+-rw-r--r--   0 cekk       (501) staff       (20)     1403 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/boolean.js
+-rw-r--r--   0 cekk       (501) staff       (20)     6227 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/date.js
+-rw-r--r--   0 cekk       (501) staff       (20)     2137 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1570 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/select.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.630091 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/LocationFilter/
+-rw-r--r--   0 cekk       (501) staff       (20)     3402 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/LocationFilter/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.630389 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     7281 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.630665 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchFilters/
+-rw-r--r--   0 cekk       (501) staff       (20)     3263 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchFilters/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.631576 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.632389 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/
+-rw-r--r--   0 cekk       (501) staff       (20)     3647 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/Bando.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1440 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/DateAndPosition.js
+-rw-r--r--   0 cekk       (501) staff       (20)     7462 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/ResultItem.js
+-rw-r--r--   0 cekk       (501) staff       (20)     3160 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/header.js
+-rw-r--r--   0 cekk       (501) staff       (20)     2531 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1726 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/pagination.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.632674 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchableTextFilter/
+-rw-r--r--   0 cekk       (501) staff       (20)     2703 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchableTextFilter/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.633199 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SpecificFilters/
+-rw-r--r--   0 cekk       (501) staff       (20)     7415 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SpecificFilters/SpecificFilter.js
+-rw-r--r--   0 cekk       (501) staff       (20)     2177 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SpecificFilters/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)      529 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.634766 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)     1398 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/apiFetch.js
+-rw-r--r--   0 cekk       (501) staff       (20)      690 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/i18n.js
+-rw-r--r--   0 cekk       (501) staff       (20)      660 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/icons.js
+-rw-r--r--   0 cekk       (501) staff       (20)      375 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/searchContext.js
+-rw-r--r--   0 cekk       (501) staff       (20)     3249 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/types.js
+-rw-r--r--   0 cekk       (501) staff       (20)      933 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/vocabulary.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.635375 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.635640 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/Pagination/
+-rw-r--r--   0 cekk       (501) staff       (20)      217 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/Pagination/pagination.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.635903 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchFilters/
+-rw-r--r--   0 cekk       (501) staff       (20)     5251 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchFilters/filters.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.636792 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchResults/
+-rw-r--r--   0 cekk       (501) staff       (20)      539 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchResults/header.less
+-rw-r--r--   0 cekk       (501) staff       (20)      114 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchResults/loading.less
+-rw-r--r--   0 cekk       (501) staff       (20)     3059 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchResults/result_item.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.637048 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SpecificFilters/
+-rw-r--r--   0 cekk       (501) staff       (20)     1212 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SpecificFilters/specific_filters.less
+-rw-r--r--   0 cekk       (501) staff       (20)      304 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/generic.less
+-rw-r--r--   0 cekk       (501) staff       (20)      884 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/index.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.637561 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     1716 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/templates/search.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1722 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/browser/templates/search_local.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2110 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.638875 rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/
+-rw-r--r--   0 cekk       (501) staff       (20)      549 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      267 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/additional_templates.py
+-rw-r--r--   0 cekk       (501) staff       (20)      346 2023-06-27 12:29:54.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/custom_filters.py
+-rw-r--r--   0 cekk       (501) staff       (20)      282 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/layer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4881 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/settings.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.639891 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.610586 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.640430 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     4576 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     8390 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.610851 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.640943 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     5079 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     8806 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1460 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     6682 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/rer.sitesearch.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1777 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      498 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/locales/update.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.611349 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.642542 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      142 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      507 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      240 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       98 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      250 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/rolemap.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/default/sitesearch_various.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.643045 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/to_4000/
+-rw-r--r--   0 cekk       (501) staff       (20)      274 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/to_4000/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     1399 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/to_4000/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.644332 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      155 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      185 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      278 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/uninstall/cssregistry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      113 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      364 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/uninstall/skins.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.645062 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      233 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.646090 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4985 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/catalog.py
+-rw-r--r--   0 cekk       (501) staff       (20)      283 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      977 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/summary.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.646537 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      197 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.647279 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      587 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     7919 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.648119 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search_filters/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search_filters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      429 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search_filters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      519 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search_filters/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2753 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/utils.py
+-rw-r--r--   0 cekk       (501) staff       (20)      421 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2226 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.648826 rer.sitesearch-4.3.1/src/rer/sitesearch/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1951 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/tests/disabled_test_search_filters_endpoint.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2297 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)      430 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      686 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/upgrades.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      461 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/utils.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3246 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer/sitesearch/vocabularies.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:29:55.621276 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    15968 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     5956 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      139 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      218 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     2780 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/webpack.config.js
+-rw-r--r--   0 cekk       (501) staff       (20)   473980 2023-06-27 12:29:55.000000 rer.sitesearch-4.3.1/yarn.lock
```

### Comparing `rer.sitesearch-4.3.0/CHANGELOG.rst` & `rer.sitesearch-4.3.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+4.3.1 (2023-06-27)
+------------------
+
+- Fix release: do not force python version.
+  [cekk]
+
+
 4.3.0 (2023-03-30)
 ------------------
 
 - Search only content-types enabled in control-panel when using Plone catalog tool.
   [cekk]
```

### Comparing `rer.sitesearch-4.3.0/PKG-INFO` & `rer.sitesearch-4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.sitesearch
-Version: 4.3.0
+Version: 4.3.1
 Summary: A product that change the base site search of Plone with some new features.
 Home-page: https://github.com/RegioneER/rer.sitesearch
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.sitesearch
 Project-URL: Source, https://github.com/RegioneER/rer.sitesearch
@@ -189,14 +189,21 @@
         .. image:: https://avatars1.githubusercontent.com/u/1087171?s=100&v=4
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.net/
         
         Changelog
         =========
         
+        4.3.1 (2023-06-27)
+        ------------------
+        
+        - Fix release: do not force python version.
+          [cekk]
+        
+        
         4.3.0 (2023-03-30)
         ------------------
         
         - Search only content-types enabled in control-panel when using Plone catalog tool.
           [cekk]
         
         
@@ -548,9 +555,8 @@
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python
-Requires-Python: ==2.7
 Provides-Extra: test
```

### Comparing `rer.sitesearch-4.3.0/README.rst` & `rer.sitesearch-4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/docs/INSTALL.txt` & `rer.sitesearch-4.3.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/docs/LICENSE.GPL` & `rer.sitesearch-4.3.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/docs/LICENSE.txt` & `rer.sitesearch-4.3.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/docs/SiteSearch_Configurazione.JPG` & `rer.sitesearch-4.3.1/docs/SiteSearch_Configurazione.JPG`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/docs/SiteSearch_Risultati-ricerca.JPG` & `rer.sitesearch-4.3.1/docs/SiteSearch_Risultati-ricerca.JPG`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/docs/rer-logo.png` & `rer.sitesearch-4.3.1/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/package.json` & `rer.sitesearch-4.3.1/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987980769230769%*

 * *Differences: {"'dependencies'": "{'moment': '^2.29.4'}"}*

```diff
@@ -5,15 +5,15 @@
         "@fortawesome/free-solid-svg-icons": "^5.15.1",
         "@fortawesome/react-fontawesome": "^0.1.12",
         "array-move": "^3.0.1",
         "axios": "^0.21.2",
         "dataobject-parser": "^1.2.1",
         "date-fns": "^2.16.1",
         "lodash.debounce": "^4.0.8",
-        "moment": "^2.29.1",
+        "moment": "^2.29.4",
         "plone-less-base": "git+https://git@github.com/RedTurtle/plone-less-base#master",
         "query-string": "^6.13.7",
         "react": "^16.8.5",
         "react-day-picker": "^7.4.8",
         "react-dom": "^16.8.5",
         "react-paginate": "^6.5.0",
         "react-select": "^3.0.3"
```

### Comparing `rer.sitesearch-4.3.0/setup.py` & `rer.sitesearch-4.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "4.3.0"
+version = "4.3.1"
 
 setup(
     name="rer.sitesearch",
     version=version,
     description="A product that change the base site search of Plone with some new features.",
     long_description=open("README.rst").read() + "\n" + open("CHANGELOG.rst").read(),
     # Get more strings from
@@ -30,15 +30,14 @@
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["rer"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "plone.api>=1.8.4",
         "plone.restapi",
         "plone.app.dexterity",
         "collective.z3cform.jsonwidget",
```

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/custom_filters.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/custom_filters.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/adapters/permission_checker.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/adapters/permission_checker.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/configure.zcml` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/controlpanel.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/i18n.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/i18n.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/search.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/search.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.css` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.css.map` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/dist/prod/main.js.map` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/dist/prod/main.js.map`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/GroupsFilter/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/GroupsFilter/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/boolean.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/boolean.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/date.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/date.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/IndexesFilters/select.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/IndexesFilters/select.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/LocationFilter/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/LocationFilter/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchContainer/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchContainer/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchFilters/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchFilters/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/Bando.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/Bando.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/DateAndPosition.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/DateAndPosition.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/ResultItem.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/ResultItem/ResultItem.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/header.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/header.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchResults/pagination.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchResults/pagination.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SearchableTextFilter/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SearchableTextFilter/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SpecificFilters/SpecificFilter.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SpecificFilters/SpecificFilter.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/SpecificFilters/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/SpecificFilters/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/index.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/index.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/apiFetch.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/apiFetch.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/i18n.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/icons.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/icons.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/types.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/types.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/js/utils/vocabulary.js` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/js/utils/vocabulary.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchFilters/filters.less` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchFilters/filters.less`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchResults/header.less` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchResults/header.less`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SearchResults/result_item.less` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SearchResults/result_item.less`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/SpecificFilters/specific_filters.less` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/SpecificFilters/specific_filters.less`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/static/styles/index.less` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/static/styles/index.less`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/templates/search.pt` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/templates/search.pt`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/browser/templates/search_local.pt` & `rer.sitesearch-4.3.1/src/rer/sitesearch/browser/templates/search_local.pt`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/configure.zcml` & `rer.sitesearch-4.3.1/src/rer/sitesearch/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/__init__.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/interfaces/settings.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.mo` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.mo`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.po` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/en/LC_MESSAGES/rer.sitesearch.po`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.mo` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.mo`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.po` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/it/LC_MESSAGES/rer.sitesearch.po`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/manual.pot` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/rer.sitesearch.pot` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/rer.sitesearch.pot`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/locales/update.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/profiles/to_4000/registry.xml` & `rer.sitesearch-4.3.1/src/rer/sitesearch/profiles/to_4000/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/catalog.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/catalog.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/serializer/summary.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/serializer/summary.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search/configure.zcml` & `rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search/get.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search/get.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/services/search_filters/get.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/services/search_filters/get.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/restapi/utils.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/restapi/utils.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/testing.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/testing.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/tests/disabled_test_search_filters_endpoint.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/tests/disabled_test_search_filters_endpoint.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/tests/test_setup.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/upgrades.zcml` & `rer.sitesearch-4.3.1/src/rer/sitesearch/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer/sitesearch/vocabularies.py` & `rer.sitesearch-4.3.1/src/rer/sitesearch/vocabularies.py`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/PKG-INFO` & `rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.sitesearch
-Version: 4.3.0
+Version: 4.3.1
 Summary: A product that change the base site search of Plone with some new features.
 Home-page: https://github.com/RegioneER/rer.sitesearch
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.sitesearch
 Project-URL: Source, https://github.com/RegioneER/rer.sitesearch
@@ -189,14 +189,21 @@
         .. image:: https://avatars1.githubusercontent.com/u/1087171?s=100&v=4
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.net/
         
         Changelog
         =========
         
+        4.3.1 (2023-06-27)
+        ------------------
+        
+        - Fix release: do not force python version.
+          [cekk]
+        
+        
         4.3.0 (2023-03-30)
         ------------------
         
         - Search only content-types enabled in control-panel when using Plone catalog tool.
           [cekk]
         
         
@@ -548,9 +555,8 @@
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python
-Requires-Python: ==2.7
 Provides-Extra: test
```

### Comparing `rer.sitesearch-4.3.0/src/rer.sitesearch.egg-info/SOURCES.txt` & `rer.sitesearch-4.3.1/src/rer.sitesearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/webpack.config.js` & `rer.sitesearch-4.3.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `rer.sitesearch-4.3.0/yarn.lock` & `rer.sitesearch-4.3.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2788,17 +2788,17 @@
   version "2.1.1"
   resolved "https://registry.yarnpkg.com/bser/-/bser-2.1.1.tgz#e6787da20ece9d07998533cfd9de6f5c38f4bc05"
   integrity sha512-gQxTNE/GAfIIrmHLUE3oJyp5FO6HRBfhjnw4/wMmA63ZGDJnWBmgY/lyQBpnDUkGmAhbSe39tx2d/iTOAfglwQ==
   dependencies:
     node-int64 "^0.4.0"
 
 buffer-from@^1.0.0:
-  version "1.1.1"
-  resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.1.tgz#32713bc028f75c02fdb710d7c7bcec1f2c6070ef"
-  integrity sha512-MQcXEUbCKtEo7bhqEs6560Hyd4XaovZlO/k9V3hjVUF/zwW7KBVdSK4gIt/bzwS9MbR5qob+F5jusZsb0YQK2A==
+  version "1.1.2"
+  resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
+  integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
 buffer-indexof@^1.0.0:
   version "1.1.1"
   resolved "https://registry.yarnpkg.com/buffer-indexof/-/buffer-indexof-1.1.1.tgz#52fabcc6a606d1a00302802648ef68f639da268c"
   integrity sha512-4/rOEg86jivtPTeOUUT61jJO1Ya1TrR/OkqCSZDyq84WJh3LuuiphBYJN+fm5xufIk4XAFcEwte/8WzC8If/1g==
 
 buffer-xor@^1.0.3:
@@ -4387,17 +4387,17 @@
 
 events@^3.0.0:
   version "3.2.0"
   resolved "https://registry.yarnpkg.com/events/-/events-3.2.0.tgz#93b87c18f8efcd4202a461aec4dfc0556b639379"
   integrity sha512-/46HWwbfCX2xTawVfkKLGxMifJYQBWMwY1mjywRtb4c9x8l5NP3KoJtnIOiL1hfdRkIuYhETxQlo62IF8tcnlg==
 
 eventsource@^1.0.7:
-  version "1.0.7"
-  resolved "https://registry.yarnpkg.com/eventsource/-/eventsource-1.0.7.tgz#8fbc72c93fcd34088090bc0a4e64f4b5cee6d8d0"
-  integrity sha512-4Ln17+vVT0k8aWq+t/bF5arcS3EpT9gYtW66EPacdj/mAFevznsnyoHLPy2BA8gbIQeIHoPsvwmfBftfcG//BQ==
+  version "1.1.1"
+  resolved "https://registry.yarnpkg.com/eventsource/-/eventsource-1.1.1.tgz#4544a35a57d7120fba4fa4c86cb4023b2c09df2f"
+  integrity sha512-qV5ZC0h7jYIAOhArFJgSfdyz6rALJyb270714o7ZtNnw2WSJ+eexhKtE0O8LYPRsHZHf2osHKZBxGPvm3kPkCA==
   dependencies:
     original "^1.0.0"
 
 evp_bytestokey@^1.0.0, evp_bytestokey@^1.0.3:
   version "1.0.3"
   resolved "https://registry.yarnpkg.com/evp_bytestokey/-/evp_bytestokey-1.0.3.tgz#7fcbdb198dc71959432efe13842684e0525acb02"
   integrity sha512-/f2Go4TognH/KvCISP7OUsHn85hT9nUkxxA9BEWxFn+Oj9o8ZNLm/40hdlgSLyuOimsrTKLUMEorQexp/aPQeA==
@@ -4757,17 +4757,17 @@
   resolved "https://registry.yarnpkg.com/flush-write-stream/-/flush-write-stream-1.1.1.tgz#8dd7d873a1babc207d94ead0c2e0e44276ebf2e8"
   integrity sha512-3Z4XhFZ3992uIq0XOqb9AreonueSYphE6oYbpt5+3u06JWklbsPkNv3ZKkP9Bz/r+1MWCaMoSQ28P85+1Yc77w==
   dependencies:
     inherits "^2.0.3"
     readable-stream "^2.3.6"
 
 follow-redirects@^1.0.0, follow-redirects@^1.14.0:
-  version "1.14.7"
-  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.14.7.tgz#2004c02eb9436eee9a21446a6477debf17e81685"
-  integrity sha512-+hbxoLbFMbRKDwohX8GkTataGqO6Jb7jGwpAlwgy2bIz25XtRm7KEzJM76R1WiNT5SwZkX4Y75SwBolkpmE7iQ==
+  version "1.14.8"
+  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.14.8.tgz#016996fb9a11a100566398b1c6839337d7bfa8fc"
+  integrity sha512-1x0S9UVJHsQprFcEC/qnNzBLcIxsjAV905f/UkQxbclCsoTWlacCNOpQa/anodLl2uaEKFhfWOvM2Qg77+15zA==
 
 for-in@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/for-in/-/for-in-1.0.2.tgz#81068d295a8142ec0ac726c6e2200c30fb6d5e80"
   integrity sha1-gQaNKVqBQuwKxybG4iAMMPttXoA=
 
 forever-agent@~0.6.1:
@@ -6992,17 +6992,17 @@
   resolved "https://registry.yarnpkg.com/minimist-options/-/minimist-options-3.0.2.tgz#fba4c8191339e13ecf4d61beb03f070103f3d954"
   integrity sha512-FyBrT/d0d4+uiZRbqznPXqw3IpZZG3gl3wKWiX784FycUKVwBt0uLBFkQrtE4tZOrgo78nZp2jnKz3L65T5LdQ==
   dependencies:
     arrify "^1.0.1"
     is-plain-obj "^1.1.0"
 
 minimist@^1.1.1, minimist@^1.2.0, minimist@^1.2.5:
-  version "1.2.5"
-  resolved "https://registry.yarnpkg.com/minimist/-/minimist-1.2.5.tgz#67d66014b66a6a8aaa0c083c5fd58df4e4e97602"
-  integrity sha512-FM9nNUYrRBAELZQT3xeZQ7fmMOBg6nWNmJKTcgsJeaLstP/UODVpGsr5OhXhhXg6f+qtJ8uiZ+PUxkDWcgIXLw==
+  version "1.2.8"
+  resolved "https://registry.yarnpkg.com/minimist/-/minimist-1.2.8.tgz#c1a464e7693302e082a075cee0c057741ac4772c"
+  integrity sha512-2yyAR8qBkN3YuheJanUpWC5U3bb5osDywNB8RzDVlDwDHbocAJveqqj1u8+SVD7jkWT4yvsHCpWqqWqAxb0zCA==
 
 mississippi@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/mississippi/-/mississippi-3.0.0.tgz#ea0a3291f97e0b5e8776b363d5f0a12d94c67022"
   integrity sha512-x471SsVjUtBRtcvd4BzKE9kFC+/2TeWgKCgw0bZcw1b9l2X3QX5vCWgF+KaZaYm87Ss//rHnWryupDrgLvmSkA==
   dependencies:
     concat-stream "^1.5.0"
@@ -7027,18 +7027,18 @@
 mkdirp@^0.5.1, mkdirp@^0.5.3, mkdirp@^0.5.5, mkdirp@~0.5.1:
   version "0.5.5"
   resolved "https://registry.yarnpkg.com/mkdirp/-/mkdirp-0.5.5.tgz#d91cefd62d1436ca0f41620e251288d420099def"
   integrity sha512-NKmAlESf6jMGym1++R0Ra7wvhV+wFW63FaSOFPwRahvea0gMUcGUhVeAg/0BC0wiv9ih5NYPB1Wn1UEI1/L+xQ==
   dependencies:
     minimist "^1.2.5"
 
-moment@^2.29.1:
-  version "2.29.1"
-  resolved "https://registry.yarnpkg.com/moment/-/moment-2.29.1.tgz#b2be769fa31940be9eeea6469c075e35006fa3d3"
-  integrity sha512-kHmoybcPV8Sqy59DwNDY3Jefr64lK/by/da0ViFcuA4DH0vQg5Q6Ze5VimxkfQNSC+Mls/Kx53s7TjP1RhFEDQ==
+moment@^2.29.4:
+  version "2.29.4"
+  resolved "https://registry.yarnpkg.com/moment/-/moment-2.29.4.tgz#3dbe052889fe7c1b2ed966fcb3a77328964ef108"
+  integrity sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==
 
 move-concurrently@^1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/move-concurrently/-/move-concurrently-1.0.1.tgz#be2c005fda32e0b29af1f05d7c4b33214c701f92"
   integrity sha1-viwAX9oy4LKa8fBdfEszIUxwH5I=
   dependencies:
     aproba "^1.1.1"
@@ -9402,17 +9402,17 @@
   version "0.4.18"
   resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.4.18.tgz#0286a6de8be42641338594e97ccea75f0a2c585f"
   integrity sha512-try0/JqxPLF9nOjvSta7tVondkP5dwgyLDjVoyMDlmjugT2lRZ1OfsrYTkCd2hkDnJTKRbO/Rl3orm8vlsUzbA==
   dependencies:
     source-map "^0.5.6"
 
 source-map-support@^0.5.6, source-map-support@~0.5.12:
-  version "0.5.19"
-  resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.5.19.tgz#a98b62f86dcaf4f67399648c085291ab9e8fed61"
-  integrity sha512-Wonm7zOCIJzBGQdB+thsPar0kYuCIzYvxZwlBa87yi/Mdjv7Tip2cyVbLj5o0cFPN4EVkuTwb3GDDyUx2DGnGw==
+  version "0.5.21"
+  resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.5.21.tgz#04fe7c7f9e1ed2d662233c28cb2b35b9f63f6e4f"
+  integrity sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==
   dependencies:
     buffer-from "^1.0.0"
     source-map "^0.6.0"
 
 source-map-url@^0.4.0:
   version "0.4.0"
   resolved "https://registry.yarnpkg.com/source-map-url/-/source-map-url-0.4.0.tgz#3e935d7ddd73631b97659956d55128e87b5084a3"
@@ -9986,17 +9986,17 @@
     serialize-javascript "^4.0.0"
     source-map "^0.6.1"
     terser "^4.1.2"
     webpack-sources "^1.4.0"
     worker-farm "^1.7.0"
 
 terser@^4.1.2:
-  version "4.8.0"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-4.8.0.tgz#63056343d7c70bb29f3af665865a46fe03a0df17"
-  integrity sha512-EAPipTNeWsb/3wLPeup1tVPaXfIaU68xMnVdPafIL1TV05OhASArYyIfFvnvJCNrR2NIOvDVNNTFRa+Re2MWyw==
+  version "4.8.1"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-4.8.1.tgz#a00e5634562de2239fd404c649051bf6fc21144f"
+  integrity sha512-4GnLC0x667eJG0ewJTa6z/yXrbLGv80D9Ru6HIpCQmO+Q4PfEtBFi0ObSckqwL6VyQv/7ENJieXHo2ANmdQwgw==
   dependencies:
     commander "^2.20.0"
     source-map "~0.6.1"
     source-map-support "~0.5.12"
 
 test-exclude@^5.2.3:
   version "5.2.3"
@@ -10378,17 +10378,17 @@
 
 urix@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/urix/-/urix-0.1.0.tgz#da937f7a62e21fec1fd18d49b35c2935067a6c72"
   integrity sha1-2pN/emLiH+wf0Y1Js1wpNQZ6bHI=
 
 url-parse@^1.4.3:
-  version "1.5.3"
-  resolved "https://registry.yarnpkg.com/url-parse/-/url-parse-1.5.3.tgz#71c1303d38fb6639ade183c2992c8cc0686df862"
-  integrity sha512-IIORyIQD9rvj0A4CLWsHkBBJuNqWpFQe224b6j9t/ABmquIS0qDU2pY6kl6AuOrL5OkCXHMCFNe1jBcuAggjvQ==
+  version "1.5.10"
+  resolved "https://registry.yarnpkg.com/url-parse/-/url-parse-1.5.10.tgz#9d3c2f736c1d75dd3bd2be507dcc111f1e2ea9c1"
+  integrity sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==
   dependencies:
     querystringify "^2.1.1"
     requires-port "^1.0.0"
 
 url@^0.11.0:
   version "0.11.0"
   resolved "https://registry.yarnpkg.com/url/-/url-0.11.0.tgz#3838e97cfc60521eb73c525a8e55bfdd9e2e28f1"
```

