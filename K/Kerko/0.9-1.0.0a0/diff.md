# Comparing `tmp/Kerko-0.9.tar.gz` & `tmp/Kerko-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kerko-0.9.tar", last modified: Fri Dec 30 00:26:47 2022, max compression
+gzip compressed data, was "Kerko-1.0.0a0.tar", last modified: Tue Jun 27 00:18:43 2023, max compression
```

## Comparing `Kerko-0.9.tar` & `Kerko-1.0.0a0.tar`

### file list

```diff
@@ -1,191 +1,216 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.826945 Kerko-0.9/
--rw-rw-r--   0 david     (1000) david     (1000)    22503 2022-12-30 00:19:39.000000 Kerko-0.9/CHANGELOG.md
--rw-r--r--   0 david     (1000) david     (1000)    35149 2019-07-16 20:48:01.000000 Kerko-0.9/LICENSE.txt
--rw-r--r--   0 david     (1000) david     (1000)      149 2022-12-29 23:09:02.000000 Kerko-0.9/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)    72687 2022-12-30 00:26:47.826945 Kerko-0.9/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)    48322 2022-12-30 00:22:24.000000 Kerko-0.9/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      135 2020-10-30 02:39:43.000000 Kerko-0.9/babel.cfg
--rw-r--r--   0 david     (1000) david     (1000)      629 2022-10-11 23:06:43.000000 Kerko-0.9/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)     3110 2022-12-30 00:26:47.826945 Kerko-0.9/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     1336 2020-10-30 05:50:50.000000 Kerko-0.9/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/Kerko.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    72687 2022-12-30 00:26:47.000000 Kerko-0.9/src/Kerko.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     8516 2022-12-30 00:26:47.000000 Kerko-0.9/src/Kerko.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2022-12-30 00:26:47.000000 Kerko-0.9/src/Kerko.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       39 2022-12-30 00:26:47.000000 Kerko-0.9/src/Kerko.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      403 2022-12-30 00:26:47.000000 Kerko-0.9/src/Kerko.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        6 2022-12-30 00:26:47.000000 Kerko-0.9/src/Kerko.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.814945 Kerko-0.9/src/kerko/
--rw-rw-r--   0 david     (1000) david     (1000)     4628 2022-12-29 23:36:38.000000 Kerko-0.9/src/kerko/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     6288 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)     6795 2022-12-22 21:42:38.000000 Kerko-0.9/src/kerko/codecs.py
--rw-rw-r--   0 david     (1000) david     (1000)    75445 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/composer.py
--rw-rw-r--   0 david     (1000) david     (1000)     7596 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/criteria.py
--rw-rw-r--   0 david     (1000) david     (1000)     4747 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)     1294 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    25499 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/extractors.py
--rw-rw-r--   0 david     (1000) david     (1000)      517 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/forms.py
--rw-rw-r--   0 david     (1000) david     (1000)     2101 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/jinja2.py
--rw-r--r--   0 david     (1000) david     (1000)     1674 2020-12-31 21:31:13.000000 Kerko-0.9/src/kerko/renderers.py
--rw-rw-r--   0 david     (1000) david     (1000)    12863 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/searcher.py
--rw-rw-r--   0 david     (1000) david     (1000)      150 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/shortcuts.py
--rw-rw-r--   0 david     (1000) david     (1000)    27191 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/specs.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/kerko/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/kerko/static/kerko/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.814945 Kerko-0.9/src/kerko/static/kerko/css/
--rw-rw-r--   0 david     (1000) david     (1000)     1844 2022-11-04 17:41:11.000000 Kerko-0.9/src/kerko/static/kerko/css/styles.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.814945 Kerko-0.9/src/kerko/static/kerko/js/
--rw-r--r--   0 david     (1000) david     (1000)      404 2020-08-12 17:15:28.000000 Kerko-0.9/src/kerko/static/kerko/js/item.js
--rw-rw-r--   0 david     (1000) david     (1000)     1369 2020-11-04 00:45:08.000000 Kerko-0.9/src/kerko/static/kerko/js/print.js
--rw-rw-r--   0 david     (1000) david     (1000)     2259 2022-10-11 19:26:42.000000 Kerko-0.9/src/kerko/static/kerko/js/search.js
--rw-rw-r--   0 david     (1000) david     (1000)     2574 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/storage.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.814945 Kerko-0.9/src/kerko/sync/
--rw-rw-r--   0 david     (1000) david     (1000)       30 2022-06-08 13:26:49.000000 Kerko-0.9/src/kerko/sync/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4042 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/sync/attachments.py
--rw-rw-r--   0 david     (1000) david     (1000)     5301 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/sync/cache.py
--rw-rw-r--   0 david     (1000) david     (1000)     3740 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/sync/index.py
--rw-rw-r--   0 david     (1000) david     (1000)    11734 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/sync/zotero.py
--rw-rw-r--   0 david     (1000) david     (1000)     3035 2021-11-16 01:35:10.000000 Kerko-0.9/src/kerko/tags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/kerko/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.818945 Kerko-0.9/src/kerko/templates/kerko/
--rw-rw-r--   0 david     (1000) david     (1000)      155 2020-06-20 17:03:06.000000 Kerko-0.9/src/kerko/templates/kerko/_attributes.html.jinja2
--rw-r--r--   0 david     (1000) david     (1000)      632 2022-03-18 22:16:56.000000 Kerko-0.9/src/kerko/templates/kerko/_badges.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1234 2022-11-12 18:42:55.000000 Kerko-0.9/src/kerko/templates/kerko/_breadbox.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1623 2022-10-11 19:26:42.000000 Kerko-0.9/src/kerko/templates/kerko/_collapse.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      375 2022-09-30 19:58:46.000000 Kerko-0.9/src/kerko/templates/kerko/_facet_breadbox.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      560 2022-10-11 19:26:42.000000 Kerko-0.9/src/kerko/templates/kerko/_facet_field.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      281 2022-10-11 19:26:42.000000 Kerko-0.9/src/kerko/templates/kerko/_facet_search.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     6610 2022-10-11 19:26:42.000000 Kerko-0.9/src/kerko/templates/kerko/_facets.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1428 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/templates/kerko/_item-relations.html.jinja2
--rw-r--r--   0 david     (1000) david     (1000)       90 2019-07-16 20:47:42.000000 Kerko-0.9/src/kerko/templates/kerko/_navbar_brand.html.jinja2
--rw-r--r--   0 david     (1000) david     (1000)      280 2020-06-20 23:37:07.000000 Kerko-0.9/src/kerko/templates/kerko/_navbar_items.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     3908 2021-11-16 01:35:10.000000 Kerko-0.9/src/kerko/templates/kerko/_pager.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1819 2021-10-25 19:52:47.000000 Kerko-0.9/src/kerko/templates/kerko/_search-form.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    10098 2022-10-11 19:26:42.000000 Kerko-0.9/src/kerko/templates/kerko/_search-help.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      578 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/templates/kerko/_search-metas.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     5389 2022-04-06 22:19:07.000000 Kerko-0.9/src/kerko/templates/kerko/_search-result.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1228 2021-04-06 23:31:19.000000 Kerko-0.9/src/kerko/templates/kerko/_sorter.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     4284 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/templates/kerko/atom.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     2125 2021-11-16 01:35:10.000000 Kerko-0.9/src/kerko/templates/kerko/base.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    18469 2022-12-29 19:43:56.000000 Kerko-0.9/src/kerko/templates/kerko/item.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     6597 2022-12-29 23:12:47.000000 Kerko-0.9/src/kerko/templates/kerko/layout.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1700 2022-12-29 18:28:28.000000 Kerko-0.9/src/kerko/templates/kerko/search-item.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    12942 2022-12-29 23:13:27.000000 Kerko-0.9/src/kerko/templates/kerko/search.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      349 2022-06-09 00:37:21.000000 Kerko-0.9/src/kerko/templates/kerko/sitemap.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      325 2022-06-08 12:43:24.000000 Kerko-0.9/src/kerko/templates/kerko/sitemap_index.xml.jinja2
--rw-r--r--   0 david     (1000) david     (1000)      868 2019-07-16 20:47:42.000000 Kerko-0.9/src/kerko/text.py
--rw-rw-r--   0 david     (1000) david     (1000)     2579 2021-04-06 23:31:19.000000 Kerko-0.9/src/kerko/transformers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/kerko/translations/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/kerko/translations/de/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.818945 Kerko-0.9/src/kerko/translations/de/LC_MESSAGES/
--rw-r--r--   0 david     (1000) david     (1000)    18452 2022-12-30 00:26:47.000000 Kerko-0.9/src/kerko/translations/de/LC_MESSAGES/kerko.mo
--rw-r--r--   0 david     (1000) david     (1000)    26381 2020-08-11 21:34:53.000000 Kerko-0.9/src/kerko/translations/de/LC_MESSAGES/kerko.po
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.810945 Kerko-0.9/src/kerko/translations/fr/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.818945 Kerko-0.9/src/kerko/translations/fr/LC_MESSAGES/
--rw-r--r--   0 david     (1000) david     (1000)    21476 2022-12-30 00:26:47.000000 Kerko-0.9/src/kerko/translations/fr/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    31224 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/translations/fr/LC_MESSAGES/kerko.po
--rw-r--r--   0 david     (1000) david     (1000)      868 2019-07-16 20:47:42.000000 Kerko-0.9/src/kerko/tree.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.818945 Kerko-0.9/src/kerko/views/
--rw-rw-r--   0 david     (1000) david     (1000)       52 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2329 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/breadbox.py
--rw-rw-r--   0 david     (1000) david     (1000)     1660 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/item_creators.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/item_facets.py
--rw-rw-r--   0 david     (1000) david     (1000)     4155 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/item_meta.py
--rw-rw-r--   0 david     (1000) david     (1000)     2922 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/item_relations.py
--rw-rw-r--   0 david     (1000) david     (1000)     2366 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/pager.py
--rw-rw-r--   0 david     (1000) david     (1000)    17459 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/routes.py
--rw-rw-r--   0 david     (1000) david     (1000)    11540 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/search.py
--rw-rw-r--   0 david     (1000) david     (1000)      690 2022-12-29 20:19:18.000000 Kerko-0.9/src/kerko/views/sorter.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.818945 Kerko-0.9/tests/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-10-22 21:00:14.000000 Kerko-0.9/tests/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.818945 Kerko-0.9/tests/integration_testing/
--rw-rw-r--   0 david     (1000) david     (1000)     1655 2022-06-08 12:43:24.000000 Kerko-0.9/tests/integration_testing/README.md
--rw-rw-r--   0 david     (1000) david     (1000)    10827 2022-06-09 15:21:28.000000 Kerko-0.9/tests/integration_testing/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-30 00:26:47.826945 Kerko-0.9/tests/integration_testing/api_responses/
--rw-rw-r--   0 david     (1000) david     (1000)     1071 2022-06-08 03:23:01.000000 Kerko-0.9/tests/integration_testing/api_responses/collections.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2022-06-08 03:23:03.000000 Kerko-0.9/tests/integration_testing/api_responses/fulltext.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2022-06-08 03:23:04.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_artwork.json
--rw-rw-r--   0 david     (1000) david     (1000)      329 2022-06-08 03:23:04.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_audioRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2022-06-08 03:23:05.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_bill.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2022-06-08 03:23:05.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_blogPost.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2022-06-08 03:23:05.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_book.json
--rw-rw-r--   0 david     (1000) david     (1000)      498 2022-06-08 03:23:06.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_bookSection.json
--rw-rw-r--   0 david     (1000) david     (1000)      242 2022-06-08 03:23:06.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_case.json
--rw-rw-r--   0 david     (1000) david     (1000)      172 2022-06-08 03:23:07.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_computerProgram.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2022-06-08 03:23:07.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_conferencePaper.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2022-06-08 03:23:07.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_dictionaryEntry.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2022-06-08 03:23:08.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_document.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2022-06-08 03:23:08.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_email.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2022-06-08 03:23:08.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_encyclopediaArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      336 2022-06-08 03:23:09.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_film.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2022-06-08 03:23:09.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_forumPost.json
--rw-rw-r--   0 david     (1000) david     (1000)       88 2022-06-08 03:23:10.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_hearing.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2022-06-08 03:23:10.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_instantMessage.json
--rw-rw-r--   0 david     (1000) david     (1000)      347 2022-06-08 03:23:10.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_interview.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2022-06-08 03:23:11.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_journalArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2022-06-08 03:23:11.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_letter.json
--rw-rw-r--   0 david     (1000) david     (1000)      341 2022-06-08 03:23:11.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_magazineArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2022-06-08 03:23:12.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_manuscript.json
--rw-rw-r--   0 david     (1000) david     (1000)      265 2022-06-08 03:23:12.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_map.json
--rw-rw-r--   0 david     (1000) david     (1000)      341 2022-06-08 03:23:13.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_newspaperArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2022-06-08 03:23:13.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_note.json
--rw-rw-r--   0 david     (1000) david     (1000)      259 2022-06-08 03:23:13.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_patent.json
--rw-rw-r--   0 david     (1000) david     (1000)      244 2022-06-08 03:23:14.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_podcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2022-06-08 12:43:33.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_preprint.json
--rw-rw-r--   0 david     (1000) david     (1000)      170 2022-06-08 03:23:14.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_presentation.json
--rw-rw-r--   0 david     (1000) david     (1000)      495 2022-06-08 03:23:15.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_radioBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      337 2022-06-08 03:23:15.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_report.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2022-06-08 03:23:16.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_statute.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2022-06-08 03:23:16.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_thesis.json
--rw-rw-r--   0 david     (1000) david     (1000)      495 2022-06-08 03:23:16.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_tvBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      421 2022-06-08 03:23:17.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_videoRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2022-06-08 03:23:17.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeCreatorTypes_webpage.json
--rw-rw-r--   0 david     (1000) david     (1000)     1129 2022-06-08 03:23:04.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_artwork.json
--rw-rw-r--   0 david     (1000) david     (1000)     1574 2022-06-08 03:23:04.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)     1251 2022-06-08 03:23:05.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_bill.json
--rw-rw-r--   0 david     (1000) david     (1000)      803 2022-06-08 03:23:05.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_blogPost.json
--rw-rw-r--   0 david     (1000) david     (1000)     1637 2022-06-08 03:23:05.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_book.json
--rw-rw-r--   0 david     (1000) david     (1000)     1706 2022-06-08 03:23:06.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_bookSection.json
--rw-rw-r--   0 david     (1000) david     (1000)     1128 2022-06-08 03:23:06.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_case.json
--rw-rw-r--   0 david     (1000) david     (1000)     1423 2022-06-08 12:43:33.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json
--rw-rw-r--   0 david     (1000) david     (1000)     1631 2022-06-08 03:23:07.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json
--rw-rw-r--   0 david     (1000) david     (1000)     1718 2022-06-08 03:23:07.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json
--rw-rw-r--   0 david     (1000) david     (1000)     1047 2022-06-08 03:23:08.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_document.json
--rw-rw-r--   0 david     (1000) david     (1000)      649 2022-06-08 03:23:08.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_email.json
--rw-rw-r--   0 david     (1000) david     (1000)     1722 2022-06-08 03:23:08.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1284 2022-06-08 03:23:09.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_film.json
--rw-rw-r--   0 david     (1000) david     (1000)      808 2022-06-08 03:23:09.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_forumPost.json
--rw-rw-r--   0 david     (1000) david     (1000)     1338 2022-06-08 03:23:09.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_hearing.json
--rw-rw-r--   0 david     (1000) david     (1000)      645 2022-06-08 03:23:10.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json
--rw-rw-r--   0 david     (1000) david     (1000)     1050 2022-06-08 03:23:10.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_interview.json
--rw-rw-r--   0 david     (1000) david     (1000)     1711 2022-06-08 03:23:11.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1043 2022-06-08 03:23:11.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_letter.json
--rw-rw-r--   0 david     (1000) david     (1000)     1328 2022-06-08 03:23:11.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1191 2022-06-08 03:23:12.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_manuscript.json
--rw-rw-r--   0 david     (1000) david     (1000)     1471 2022-06-08 03:23:12.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_map.json
--rw-rw-r--   0 david     (1000) david     (1000)     1402 2022-06-08 03:23:12.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2022-06-08 03:23:13.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_note.json
--rw-rw-r--   0 david     (1000) david     (1000)     1532 2022-06-08 03:23:13.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_patent.json
--rw-rw-r--   0 david     (1000) david     (1000)      906 2022-06-08 03:23:13.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_podcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1560 2022-06-08 12:43:33.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_preprint.json
--rw-rw-r--   0 david     (1000) david     (1000)      872 2022-06-08 03:23:14.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_presentation.json
--rw-rw-r--   0 david     (1000) david     (1000)     1444 2022-06-08 03:23:15.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1430 2022-06-08 03:23:15.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_report.json
--rw-rw-r--   0 david     (1000) david     (1000)     1189 2022-06-08 03:23:15.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_statute.json
--rw-rw-r--   0 david     (1000) david     (1000)     1265 2022-06-08 03:23:16.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_thesis.json
--rw-rw-r--   0 david     (1000) david     (1000)     1444 2022-06-08 03:23:16.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1576 2022-06-08 03:23:16.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      809 2022-06-08 03:23:17.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_webpage.json
--rw-rw-r--   0 david     (1000) david     (1000)     2883 2022-06-08 12:43:33.000000 Kerko-0.9/tests/integration_testing/api_responses/itemTypes.json
--rw-rw-r--   0 david     (1000) david     (1000)    42561 2022-06-08 03:23:03.000000 Kerko-0.9/tests/integration_testing/api_responses/items.json
--rw-rw-r--   0 david     (1000) david     (1000)       22 2022-06-08 03:23:03.000000 Kerko-0.9/tests/integration_testing/api_responses/items_versions.json
--rwxrwxr-x   0 david     (1000) david     (1000)     2697 2022-06-08 12:43:33.000000 Kerko-0.9/tests/integration_testing/api_responses/update.bash
--rw-rw-r--   0 david     (1000) david     (1000)     8673 2022-12-29 20:19:18.000000 Kerko-0.9/tests/test_atom_feed.py
--rw-rw-r--   0 david     (1000) david     (1000)    13123 2022-12-29 20:19:18.000000 Kerko-0.9/tests/test_datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)    16760 2022-12-29 20:19:18.000000 Kerko-0.9/tests/test_item_meta.py
--rw-rw-r--   0 david     (1000) david     (1000)     4830 2022-12-29 20:19:18.000000 Kerko-0.9/tests/test_pager.py
--rw-rw-r--   0 david     (1000) david     (1000)     2514 2022-12-29 20:19:18.000000 Kerko-0.9/tests/test_sitemap.py
--rw-rw-r--   0 david     (1000) david     (1000)     1875 2022-06-08 14:01:58.000000 Kerko-0.9/tests/test_sync.py
--rw-rw-r--   0 david     (1000) david     (1000)     8126 2021-11-16 01:35:10.000000 Kerko-0.9/tests/test_tags.py
--rw-rw-r--   0 david     (1000) david     (1000)      640 2022-11-04 18:41:21.000000 Kerko-0.9/tox.ini
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/
+-rw-rw-r--   0 david     (1000) david     (1000)    28770 2023-06-27 00:15:39.000000 Kerko-1.0.0a0/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)    35149 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/LICENSE.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      215 2023-06-27 00:18:19.000000 Kerko-1.0.0a0/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)    43335 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    12613 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/babel.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)     2777 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/background.md
+-rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/changelog.md
+-rw-rw-r--   0 david     (1000) david     (1000)     7272 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/config-basics.md
+-rw-rw-r--   0 david     (1000) david     (1000)    23335 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/config-params.md
+-rw-rw-r--   0 david     (1000) david     (1000)     4040 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/contributing.md
+-rw-rw-r--   0 david     (1000) david     (1000)      885 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/deployment.md
+-rw-rw-r--   0 david     (1000) david     (1000)    14801 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/getting-started.md
+-rw-rw-r--   0 david     (1000) david     (1000)    18067 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/index.md
+-rw-rw-r--   0 david     (1000) david     (1000)     3351 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/localization.md
+-rw-rw-r--   0 david     (1000) david     (1000)     6988 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/recipes.md
+-rw-rw-r--   0 david     (1000) david     (1000)     4500 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/synchronization.md
+-rw-rw-r--   0 david     (1000) david     (1000)     1479 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/troubleshooting.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2193 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/mkdocs.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      629 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     3392 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     1336 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/Kerko.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    43335 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     9072 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       39 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      507 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        6 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/
+-rw-rw-r--   0 david     (1000) david     (1000)      962 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6433 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6795 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/codecs.py
+-rw-rw-r--   0 david     (1000) david     (1000)    36095 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/composer.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11600 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/config_helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7623 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/criteria.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4747 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18790 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/default_config.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     1294 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    26611 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/extractors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      511 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/forms.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2123 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/jinja2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1674 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/renderers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12863 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/searcher.py
+-rw-rw-r--   0 david     (1000) david     (1000)      836 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/shortcuts.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27160 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/specs.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/static/kerko/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/static/kerko/css/
+-rw-rw-r--   0 david     (1000) david     (1000)     2027 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/css/styles.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/static/kerko/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/item.js
+-rw-rw-r--   0 david     (1000) david     (1000)     1289 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/open_in_zotero.js
+-rw-rw-r--   0 david     (1000) david     (1000)     1369 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/print.js
+-rw-rw-r--   0 david     (1000) david     (1000)     2259 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/search.js
+-rw-rw-r--   0 david     (1000) david     (1000)     2564 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/storage.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/sync/
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4103 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/attachments.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5301 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/cache.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3829 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/index.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11723 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/zotero.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3035 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/tags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/templates/kerko/
+-rw-rw-r--   0 david     (1000) david     (1000)      155 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_attributes.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      632 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_badges.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1234 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_breadbox.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_collapse.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      375 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_breadbox.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      560 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_field.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_search.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     6610 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facets.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1464 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_item-relations.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_navbar_brand.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      280 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_navbar_items.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     3908 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_pager.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     4013 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_preferences.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-form.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    10118 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-help.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      578 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-metas.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     5479 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-result.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_sorter.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     4282 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/atom.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     2184 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/base.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    20615 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/item.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     6640 2023-06-26 23:55:07.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/layout.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/search-item.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    13015 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/search.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      348 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/sitemap.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      325 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/sitemap_index.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/text.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2579 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/transformers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/de/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/
+-rw-r--r--   0 david     (1000) david     (1000)    18452 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    26381 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.po
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/fr/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 david     (1000) david     (1000)    22918 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    33607 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.po
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/pt/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/
+-rw-rw-r--   0 david     (1000) david     (1000)    20867 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    30605 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/kerko.po
+-rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/tree.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       52 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2329 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/breadbox.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/views/item/
+-rw-rw-r--   0 david     (1000) david     (1000)     1361 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1660 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/creators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/facets.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4160 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/meta.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2937 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/relations.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2399 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/pager.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17274 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/routes.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11280 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/search.py
+-rw-rw-r--   0 david     (1000) david     (1000)      690 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/sorter.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/tests/integration_testing/
+-rw-rw-r--   0 david     (1000) david     (1000)     1649 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)    10620 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/tests/integration_testing/api_responses/
+-rw-rw-r--   0 david     (1000) david     (1000)     1071 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/collections.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/fulltext.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_artwork.json
+-rw-rw-r--   0 david     (1000) david     (1000)      329 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_audioRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_bill.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_blogPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_book.json
+-rw-rw-r--   0 david     (1000) david     (1000)      498 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_bookSection.json
+-rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_case.json
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_computerProgram.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_conferencePaper.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_dictionaryEntry.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_document.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_email.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_encyclopediaArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      336 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_film.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_forumPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)       88 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_hearing.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_instantMessage.json
+-rw-rw-r--   0 david     (1000) david     (1000)      347 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_interview.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_journalArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_letter.json
+-rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_magazineArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_manuscript.json
+-rw-rw-r--   0 david     (1000) david     (1000)      265 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_map.json
+-rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_newspaperArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_note.json
+-rw-rw-r--   0 david     (1000) david     (1000)      259 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_patent.json
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_podcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_preprint.json
+-rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_presentation.json
+-rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_radioBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      337 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_report.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_statute.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_thesis.json
+-rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_tvBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      421 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_videoRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_webpage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_artwork.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1574 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1251 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bill.json
+-rw-rw-r--   0 david     (1000) david     (1000)      803 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_blogPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1637 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_book.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1706 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bookSection.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1128 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_case.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1423 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1718 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1047 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_document.json
+-rw-rw-r--   0 david     (1000) david     (1000)      649 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_email.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1722 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1284 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_film.json
+-rw-rw-r--   0 david     (1000) david     (1000)      808 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_forumPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1338 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_hearing.json
+-rw-rw-r--   0 david     (1000) david     (1000)      645 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1050 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_interview.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1711 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_letter.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_manuscript.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1471 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_map.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1402 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_note.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1532 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_patent.json
+-rw-rw-r--   0 david     (1000) david     (1000)      906 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_podcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1560 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_preprint.json
+-rw-rw-r--   0 david     (1000) david     (1000)      872 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_presentation.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1430 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_report.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_statute.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1265 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_thesis.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1576 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      809 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_webpage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypes.json
+-rw-rw-r--   0 david     (1000) david     (1000)    42561 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/items.json
+-rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/items_versions.json
+-rwxrwxr-x   0 david     (1000) david     (1000)     2577 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/update.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     8683 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_atom_feed.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5321 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_config.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13271 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16760 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_item_meta.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4919 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_pager.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_sitemap.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1863 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_sync.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8126 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_tags.py
+-rw-rw-r--   0 david     (1000) david     (1000)      640 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tox.ini
```

### Comparing `Kerko-0.9/CHANGELOG.md` & `Kerko-1.0.0a0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,122 @@
 # Changelog
 
-## Latest (unreleased)
+For changes that might be specific to KerkoApp, please refer to the [KerkoApp
+changelog](https://github.com/whiskyechobravo/kerkoapp/blob/master/CHANGELOG.md).
 
-TBD.
+
+## 1.0.0alpha0
+
+*Warning:* Upgrading from version 0.9 or earlier will require that you adapt
+your installation and configuration (if you are using KerkoApp, make sure to
+check its changelog), then rebuild your search index. Use the following
+commands, then restart the application:
+
+```bash
+flask kerko clean index
+flask kerko sync index
+```
+
+Features:
+
+- Add many new configuration parameters. Please refer to the configuration
+  parameters documentation for the full list.
+- Add optional "Open in Zotero" and "View on zotero.org" buttons to item pages.
+  These are disabled by default (see the new settings `KERKO_OPEN_IN_ZOTERO_APP`
+  and `KERKO_OPEN_IN_ZOTERO_WEB`). Even when these settings are enabled, a user
+  who wishes to use such button must first enable it from the (also
+  new) Preferences dialog.
+- Add API for retrieving information about the last synchronization from Zotero.
+- Add the `kerko config` command to the Flask command line interface for
+  displaying all configuration parameters.
+
+Other changes:
+
+- Restructure and expand documentation into a unified documentation site for
+  both Kerko and KerkoApp.
+- Add Portuguese translation. Thanks to Gonçalo Cordeiro.
+
+Backwards incompatible changes:
+
+- Raise the minimum required versions of Flask, Flask-Babel, Bootstrap-Flask,
+  and WTForms. If you have a custom application, some of those may introduce
+  breaking changes.
+- The data directory has a new default location relative to the instance path.
+  Please check the documentation for the `DATA_PATH` and `INSTANCE_PATH`
+  configuration parameters. You may need to set one or both of those parameters,
+  and/or move your existing data directory.
+- Almost all configuration parameters have been renamed and/or moved into a
+  hierarchical structure. Hierarchical parameters are referred to using
+  path-like, dot-separated parameter names, and may conveniently be set with the
+  `kerko.config_helpers.config_set()` function. Here is a mapping of the changed
+  parameters:
+    - `KERKO_BOOTSTRAP_VERSION` → `kerko.assets.bootstrap_version`
+    - `KERKO_CSL_STYLE` → `kerko.zotero.csl_style`
+    - `KERKO_COMPOSER` → `kerko_composer`
+    - `KERKO_DATA_DIR` → `DATA_PATH`. Now optional, relative to the instance
+      path, and defaulting to `kerko` instead of `data/kerko`.
+    - `KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW` → `kerko.features.download_attachment_new_window`
+    - `KERKO_DOWNLOAD_CITATIONS_LINK` → `kerko.features.download_citations_link`
+    - `KERKO_DOWNLOAD_CITATIONS_MAX_COUNT` → `kerko.features.download_citations_max_count`
+    - `KERKO_FEEDS` → `kerko.feeds.formats`
+    - `KERKO_FEEDS_FIELDS` → `kerko.feeds.fields`
+    - `KERKO_FEEDS_MAX_DAYS` → `kerko.feeds.max_days`
+    - `KERKO_FEEDS_REJECT_ANY` → `kerko.feeds.reject_any`
+    - `KERKO_FEEDS_REQUIRE_ANY` → `kerko.feeds.require_any`
+    - `KERKO_FULLTEXT_SEARCH` → `kerko.search.fulltext`
+    - `KERKO_HIGHWIREPRESS_TAGS` → `kerko.meta.highwirepress_tags`
+    - `KERKO_JQUERY_VERSION` → `kerko.assets.jquery_version`
+    - `KERKO_OPEN_IN_ZOTERO_APP` → `kerko.features.open_in_zotero_app`
+    - `KERKO_OPEN_IN_ZOTERO_WEB` → `kerko.features.open_in_zotero_web`
+    - `KERKO_PAGE_LEN` → `kerko.pagination.page_len`
+    - `KERKO_PAGER_LINKS` → `kerko.pagination.pager_links`
+    - `KERKO_POPPER_VERSION` → `kerko.assets.popper_version`
+    - `KERKO_PRINT_CITATIONS_LINK` → `kerko.features.print_citations_link`
+    - `KERKO_PRINT_CITATIONS_MAX_COUNT` → `kerko.features.print_citations_max_count`
+    - `KERKO_PRINT_ITEM_LINK` → `kerko.features.print_item_link`
+    - `KERKO_RELATIONS_INITIAL_LIMIT` → `kerko.features.relations_initial_limit`
+    - `KERKO_RELATIONS_LINKS` → `kerko.features.relations_links`
+    - `KERKO_RELATIONS_SORT` → `kerko.features.relations_sort`
+    - `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH` → `kerko.features.results_abstracts_max_length`
+    - `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH_LEEWAY` → `kerko.features.results_abstracts_max_length_leeway`
+    - `KERKO_RESULTS_ABSTRACTS` → `kerko.features.results_abstracts`
+    - `KERKO_RESULTS_ABSTRACTS_TOGGLER` → `kerko.features.results_abstracts_toggler`
+    - `KERKO_RESULTS_ATTACHMENT_LINKS` → `kerko.features.results_attachment_links`
+    - `KERKO_RESULTS_FIELDS` → `kerko.search.result_fields`
+    - `KERKO_RESULTS_URL_LINKS` → `kerko.features.results_url_links`
+    - `KERKO_TEMPLATE_ATOM_FEED` → `kerko.templates.atom_feed`
+    - `KERKO_TEMPLATE_BASE` → `kerko.templates.base`
+    - `KERKO_TEMPLATE_ITEM` → `kerko.templates.item`
+    - `KERKO_TEMPLATE_LAYOUT` → `kerko.templates.layout`
+    - `KERKO_TEMPLATE_SEARCH` → `kerko.templates.search`
+    - `KERKO_TEMPLATE_SEARCH_ITEM` → `kerko.templates.search_item`
+    - `KERKO_TITLE` → `kerko.meta.title`
+    - `KERKO_WHOOSH_LANGUAGE` → `kerko.search.whoosh_language`
+    - `KERKO_WITH_JQUERY` → `kerko.assets.with_jquery`
+    - `KERKO_WITH_POPPER` → `kerko.assets.with_popper`
+    - `KERKO_ZOTERO_API_KEY` → `ZOTERO_API_KEY`
+    - `KERKO_ZOTERO_BATCH_SIZE` → `kerko.zotero.batch_size`
+    - `KERKO_ZOTERO_LIBRARY_ID` → `ZOTERO_LIBRARY_ID`
+    - `KERKO_ZOTERO_LIBRARY_TYPE` → `ZOTERO_LIBRARY_TYPE`
+    - `KERKO_ZOTERO_LOCALE` → `kerko.zotero.locale`
+    - `KERKO_ZOTERO_MAX_ATTEMPTS` → `kerko.zotero.max_attempts`
+    - `KERKO_ZOTERO_WAIT` → `kerko.zotero.wait`
+- `Composer.__init__()` now only takes a configuration object as argument
+  instead of a bunch of arguments. Thus, the initial values of the `Composer`
+  instance now depend solely on the configuration.
+- Remove the `KERKO_USE_TRANSLATIONS` configuration variable. Kerko now relies
+  on the application's default Babel domain and translation directories. Custom
+  applications that wish to load Kerko's translations should now add
+  `kerko.TRANSLATION_DOMAIN` and `kerko.TRANSLATION_DIRECTORIES` to their Babel
+  configuration.
+- The `__init__()` method of `FacetSpec` and its subclasses now only accept
+  keyword arguments.
+- The `sort_key` argument to `FacetSpec.__init__()` is now `sort_by`.
+- `Composer` built-in fields `z_dateAdded` and `z_dateModified` are now named
+  `date_added` and `date_modified` respectively.
 
 
 ## 0.9 (2022-12-29)
 
 *Warning:* Upgrading from version 0.8.x or earlier will require that you rebuild
 your search index. Use the following commands, then restart the application:
 
@@ -16,15 +126,15 @@
 ```
 
 Features:
 
 - Add expand/collapse actions on facet values, allowing full exploration of
   hierarchical facets without changing the current search.
 - Add an optional initial limit on the number of values to show under each
-  facet. When the initial limit is reached, a "show more" button allow to user
+  facet. When the initial limit is reached, a "show more" button allows the user
   to expand the full list.
 - Add Atom syndication feeds.
 - Allow searching items by their Zotero key.
 - Add XML sitemap.
 - Add the `kerko count` CLI command (mostly meant for development purposes).
 
 Bug fixes:
@@ -46,25 +156,24 @@
   to the right of the checkbox).
 - Add link to full bibliography from item pages.
 - Add blocks in templates to facilitate theming.
 - Remove `page` parameter from pagination links when `page=1`.
 - Improve documentation.
 - Make sync and schema-related error messages more helpful and user-friendly.
 - Move pydocstyle config to `pyproject.toml`.
-- Remove remnants of code aimed at Python versions older than 3.7.
-- Remove support for configuration variables `KERKO_ZOTERO_START` and
-  `KERKO_ZOTERO_END` (were only used for development and no longer practical).
 - Tag package as compatible with Python 3.10 and 3.11.
 - Remove leftover code related to Python versions older than 3.7
 
 Backwards incompatible changes:
 
 - Remove the `KERKO_FACET_COLLAPSING` option. The new initial limit on facets
   values made this feature largely redundant.
 - Remove the `collapsible` param from the `FacetSpec` class.
+- Remove support for configuration variables `KERKO_ZOTERO_START` and
+  `KERKO_ZOTERO_END` (were only used for development and no longer practical).
 
 Changes that might break custom themes:
 
 - The HTML markup and CSS styles of expand/collapse buttons have changed.
 - The parameters of the `facet`, `facet_item`, `facet_items`, `facet_fields`
   template macros have changed.
 - The `facets-container`, `facets`, and `facets-modal-body` element ids are now
@@ -287,15 +396,15 @@
 - Fix empty HTML element taking up horizontal space when there are no badges.
 
 Other changes:
 
 - Display ISO 8601 calendar dates in a more readable format, using the
   formatting style of the locale.
 - Show a timezone abbreviation along with time of last update from Zotero.
-- Add German translation. Thanks [@mmoole](https://github.com/mmoole).
+- Add German translation. Thanks to [@mmoole](https://github.com/mmoole).
 - Fix broken "Getting started" example in README.
 - Migrate most package distribution options and metadata from `setup.py` to
   `setup.cfg`.
 - Migrate project to a `src` layout.
 - Use Flask-Babel instead of its fork Flask-BabelEx, now that is has merged the
   translation domain features from Flask-BabelEx.
```

### Comparing `Kerko-0.9/LICENSE.txt` & `Kerko-1.0.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/README.md` & `Kerko-1.0.0a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,990 +1,879 @@
+Metadata-Version: 2.1
+Name: Kerko
+Version: 1.0.0a0
+Summary: A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
+Home-page: https://github.com/whiskyechobravo/kerko
+Author: David Lesieur
+Author-email: kerko@whiskyechobravo.com
+Project-URL: Documentation, https://whiskyechobravo.github.io/kerko/
+Project-URL: Code, https://github.com/whiskyechobravo/kerko
+Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/master/CHANGELOG.md
+Project-URL: Issue tracker, https://github.com/whiskyechobravo/kerko/issues
+Keywords: academia,bibliography,bibliographies,flask,search,zotero
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Flask
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Education
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE.txt
+
 [![License](https://img.shields.io/pypi/l/kerko)][Kerko]
 [![Version](https://img.shields.io/pypi/v/kerko?color=informational)][Kerko_pypi]
 [![Tests status](https://github.com/whiskyechobravo/kerko/workflows/tests/badge.svg)][Kerko_actions]
 
+
 # Kerko
 
-[Kerko] is a web application component implemented in [Python] for the [Flask]
-framework that provides a user-friendly search and browsing interface for
-sharing a bibliography managed with the [Zotero] reference manager.
+[Kerko] is a web application component that provides a user-friendly search and
+browsing interface for sharing a bibliography managed with the [Zotero]
+reference manager.
 
 The combination of Kerko and Zotero gives you the best of both worlds: a rich
 but easy to use web interface for end-users of the bibliography, and a
 well-established and powerful bibliographic reference management tool for
 individuals or teams working on the bibliography's content.
 
-Contents:
-
-- [Kerko](#kerko)
-  - [How it works](#how-it-works)
-  - [Demo site](#demo-site)
-  - [Features](#features)
-  - [Requirements](#requirements)
-  - [Getting started](#getting-started)
-  - [Configuration variables](#configuration-variables)
-  - [Synchronization process](#synchronization-process)
-  - [Command line interface (CLI)](#command-line-interface-cli)
-  - [Known limitations](#known-limitations)
-  - [Design choices](#design-choices)
-  - [Kerko Recipes](#kerko-recipes)
-    - [Ensuring full-text indexing of your attachments in Zotero](#ensuring-full-text-indexing-of-your-attachments-in-zotero)
-    - [Providing _Cites_ and _Cited by_ relations](#providing-cites-and-cited-by-relations)
-    - [Submitting your sitemap to search engines](#submitting-your-sitemap-to-search-engines)
-  - [Translating Kerko](#translating-kerko)
-  - [Contributing](#contributing)
-    - [Reporting issues](#reporting-issues)
-    - [Making code changes](#making-code-changes)
-    - [Running the tests](#running-the-tests)
-    - [Submitting code changes](#submitting-code-changes)
-    - [Submitting a translation](#submitting-a-translation)
-    - [Supporting the project](#supporting-the-project)
-  - [Changelog](#changelog)
-  - [Project background](#project-background)
-    - [Etymology](#etymology)
-  - [Powered by Kerko](#powered-by-kerko)
-
-
-## How it works
-
-A Kerko-powered bibliography is managed using Zotero, and stored in the cloud on
-zotero.org, while Kerko itself is incorporated into an application which is
-installed on a web server. The bibliographic references may reside in a Zotero
-group library, where multiple users may collaborate to manage the content, or in
-a Zotero private library. On the web server, Kerko maintains a search index,
-which is a copy of the Zotero library that is optimized for search. When users
-interact with the web application, Kerko gets all the required data from that
-search index, without ever contacting zotero.org. It is through a scheduled
-task, which runs at regular intervals, that Kerko automatically brings its
-search index up to date by using the [Zotero Web API][Zotero_web_api] to
-retrieve the latest data from zotero.org.
-
-As a Flask [blueprint][Flask_blueprint] (a "blueprint" is Flask's term for an
-application component, similar to what some other systems might call a plugin or
-an extension), Kerko only works when incorporated into a Flask application.
-However, a sample stand-alone application is available, [KerkoApp], which is
-pre-built with Kerko and ready to be deployed on a web server. KerkoApp might
-work for you if you like the default appearance and if the provided
-configuration options are sufficient for your needs, otherwise you should
-probably consider building a custom application. In a custom application, the
-Kerko-powered bibliography might be just one section of a larger website.
-
 
 ## Demo site
 
 A [KerkoApp]-based [demo site][KerkoApp_demo] is available for you to try. You
 may also view the [Zotero library][Zotero_demo] that contains the source data
 for the demo site.
 
 
+## Powered by Kerko
+
+The following sites are powered by Kerko:
+
+- [Bibliographie francophone sur l'archivistique](https://bibliopiaf.ebsi.umontreal.ca/)
+- [Community Knowledge Open Library on English-Speaking Quebec](https://ckol.quescren.ca/)
+- [Lipedema Foundation LEGATO Lipedema Library](https://library.lipedema.org/)
+- [Open Development & Education Evidence Library](https://docs.opendeved.net/)
+- [The EdTech Hub Evidence Library](http://docs.edtechhub.org/)
+- [University of Saint Joseph Research Output](https://research.usj.edu.mo/)
+
+
 ## Features
 
-The following features are implemented in Kerko:
+The main features provided by Kerko are:
 
-- Faceted search interface: allows exploration of the bibliography both in
+- **Faceted search interface**: allows exploration of the bibliography both in
   search mode and in browsing mode, potentially suiting different user needs,
-  behaviors and abilities. For example, users with a prior idea of the topic or
-  expected results are able to enter keywords or a more complex query in a
-  search field, while those who wish to become familiar with the content of the
-  bibliography or discover new topics may choose to navigate along the proposed
-  facets, to narrow or broaden their search. Since both modes are integrated
-  into a single interface, it is possible to combine them.
-- Keyword search features:
-  - Boolean operators:
-    - `AND`: matches items that contain all specified terms. This is the default
-      relation between terms when no operator is specified, e.g., `a b` is the
-      same as `a AND b`.
-    - `OR`: matches items that contain any of the specified terms, e.g., `a OR
-      b`.
-    - `NOT`: excludes items that match the term, e.g., `NOT a`.
-    - Boolean operators must be specified in uppercase and may be translated in
-      other languages.
-  - Logical grouping (with parentheses), e.g., `(a OR b) AND c`.
-  - Sequence of words (with double quotes), e.g., `"a b c"`. The default
-    difference between word positions is 1, meaning that an item will match if
-    it contains the words next to each other, but a different maximum distance
-    may be selected (with the tilde character), e.g. `"web search"~2` allows up
-    to 1 word between `web` and `search`, meaning it could match `web site
-    search` as well as `web search`.
-  - Term boosting (with the caret), e.g., `faceted^2 search browsing^0.5`
-    specifies that `faceted` is twice as important as `search` when computing
-    the relevance score of results, while `browsing` is half as important.
-    Boosting may be applied to a logical grouping, e.g., `(a b)^3 c`.
-  - Keyword search is case-insensitive, accents are folded, and punctuation is
-    ignored. To further improve recall (albeit at the cost of precision),
-    stemming is also performed on terms from most text fields, e.g., title,
-    abstract, notes. Stemming relieves the user from having to specify all
-    variants of a word when searching, e.g., terms such as `search`, `searches`,
-    and `searching` all return the same results. The [Snowball] algorithm is
-    used for that purpose.
-  - Full-text search: the text content of PDF attachments can be searched.
-  - Scope of search: users may choose to search everywhere, in
-    author/contributor names, in titles, in all fields (i.e., in metadata and
-    notes), or in documents (i.e., in the text content of attachments).
-    Applications may provide additional choices.
-- Faceted browsing: allows filtering by topic (Zotero tag), by resource type
-  (Zotero item type), by publication year. Moreover, an application may define
+  behaviors, and abilities. For example, users with a prior idea of the topic or
+  expected results may enter keywords or a more complex query in a search field,
+  while those who wish to become familiar with the content of the bibliography
+  or discover new topics may choose to navigate along the proposed facets, to
+  narrow or broaden their search. Since both modes are integrated into a single
+  interface, it is possible to combine them.
+- **Keyword search** features:
+    - Boolean operators:
+        - `AND`: matches items that contain all specified terms. This is the default
+        relation between terms when no operator is specified, e.g., `a b` is the
+        same as `a AND b`.
+        - `OR`: matches items that contain any of the specified terms, e.g., `a OR
+        b`.
+        - `NOT`: excludes items that match the term, e.g., `NOT a`.
+        - Boolean operators must be specified in uppercase and may be translated in
+        other languages.
+    - Logical grouping (with parentheses), e.g., `(a OR b) AND c`.
+    - Sequence of words (with double quotes), e.g., `"a b c"`. The default
+        difference between word positions is 1, meaning that an item will match if
+        it contains the words next to each other, but a different maximum distance
+        may be selected (with the tilde character), e.g. `"web search"~2` allows up
+        to 1 word between `web` and `search`, meaning it could match `web site
+        search` as well as `web search`.
+    - Term boosting (with the caret), e.g., `faceted^2 search browsing^0.5`
+        specifies that `faceted` is twice as important as `search` when computing
+        the relevance score of results, while `browsing` is half as important.
+        Boosting may be applied to a logical grouping, e.g., `(a b)^3 c`.
+    - Keyword search is case-insensitive, accents are folded, and punctuation is
+        ignored. To further improve recall (albeit at the cost of precision),
+        stemming is also performed on terms from most text fields, e.g., title,
+        abstract, notes. Stemming relieves the user from having to specify all
+        variants of a word when searching, e.g., terms such as `search`, `searches`,
+        and `searching` all return the same results. The [Snowball] algorithm is
+        used for that purpose.
+    - Full-text search: the text content of PDF attachments can be searched.
+    - Scope of search: users may choose to search everywhere, in
+        author/contributor names, in titles, in all fields (i.e., in metadata and
+        notes), or in documents (i.e., in the text content of attachments).
+        Applications may provide additional choices.
+- **Faceted browsing**: allows filtering by topic (Zotero tag), by resource type
+  (Zotero item type), by publication year. Moreover, you may define additional
   facets modeled on collections and subcollections; in such case, any collection
   can be represented as a facet, and each subcollection as a value within that
   facet. By taking advantage of Zotero's ability to assign any given item to
-  multiple collections, a faceted classification scheme can be modeled
-  (including hierarchies within facets).
-- Relevance scoring: provided by the [Whoosh] library and based on the [BM25F]
-  algorithm, which determines how important a term is to a document in the
-  context of the whole collection of documents, while taking into account its
-  relation to document structure (in this regard most fields are neutral, but
-  the score is boosted when a term appears in specific fields, e.g., DOI, ISBN,
-  ISSN, title, author/contributor). Any keyword search asks the question "how
-  well does this document match this query clause?", which requires calculating
-  a relevance score for each document. Filtering with facets, on the other hand,
-  has no effect on the score because it asks "does this document match this
-  query clause?", which leads to a yes or no answer.
-- Sort options: by relevance score (only applicable with keyword search), by
+  multiple collections, a faceted classification scheme can be designed,
+  including hierarchical subdivisions within facets.
+- **Relevance scoring**: provided by the [Whoosh] library and based on the
+  [BM25F] algorithm, which determines how important a term is to a document in
+  the context of the whole collection of documents, while taking into account
+  its relation to document structure (in this regard most fields are neutral,
+  but the score is boosted when a term appears in specific fields, e.g., DOI,
+  ISBN, ISSN, title, author/contributor). Any keyword search asks the question
+  "how well does this document match this query clause?", which requires
+  calculating a relevance score for each document. Filtering with facets, on the
+  other hand, has no effect on the score because it asks "does this document
+  match this query clause?", which leads to a yes or no answer.
+- **Sort options**: by relevance score (only applicable to keyword search), by
   publication date, by author, by title.
-- Citation styles: any from the [Zotero Style Repository][Zotero_styles], or
+- **Citation styles**: any from the [Zotero Style Repository][Zotero_styles], or
   custom stylesheet defined in the [Citation Style Language][CSL] (stylesheet
   must be accessible by URL).
-- Language support: the default user interface is in English, but [some
-  translations][Kerko_translations] are provided. Additional translations may be
-  created using gettext-compatible tools; see [Translating
-  Kerko](#translating-kerko). Also to consider: locales supported by the [Zotero
-  Data Schema][Zotero_schema] (which provides the names of fields, item types
-  and author types displayed by Kerko); languages supported by Whoosh (which
-  provides the search capabilities), i.e., ar, da, nl, en, fi, fr, de, hu, it,
-  no, pt, ro, ru, es, sv, tr.
-- Responsive design: the simple default implementation works on large monitors
-  as well as on small screens. It is based on [Bootstrap].
-- Customizable front-end: applications may partly or fully replace the default
-  templates, scripts and stylesheets with their own.
-- Semantic markup: pages generated by Kerko embed HTML markup that can be
+- **Language support**: the default language of the user interface is English,
+  but [some translations][Kerko_translations] are provided. Additional
+  translations may be created using gettext-compatible tools. Also to consider:
+  locales supported by the [Zotero Data Schema][Zotero_schema] (which provides
+  the names of fields, item types and author types displayed by Kerko);
+  languages supported by Whoosh (which provides the search capabilities), i.e.,
+  ar, da, nl, en, fi, fr, de, hu, it, no, pt, ro, ru, es, sv, tr.
+- **Semantic markup**: pages generated by Kerko embed HTML markup that can be
   detected by web crawlers (helping the indexing of your records by search
   engines) or by web browsers (allowing users of reference management tools to
   easily import metadata in their library). Supported schemes are:
     - [OpenURL COinS][COinS], in search results pages and individual
       bibliographic record pages. COinS is recognized by [many reference
       management tools][COinS_clients], including the [Zotero
       Connector][Zotero_Connector] browser extension.
     - Highwire Press tags, in the individual bibliographic record pages of book,
       conference paper, journal article, report or thesis items. These tags are
       recommended for indexing by [Google Scholar][HighwirePress_Google], and
       are recognized by many other databases and reference management tools,
       including the [Zotero Connector][Zotero_Connector] browser extension.
-- Web feeds: users of news aggregators or feed readers may get updates when new
-  bibliographic records are added. They may subscribe to the main feed, or to
-  one or more custom feeds.
+- **Web feeds**: users of news aggregators or feed readers may get updates when
+  new bibliographic records are added. They may subscribe to the main feed, or
+  to one or more custom feeds.
     - The main feed lists the most recently added bibliographic records.
     - Any search page has a related custom feed that lists the most recently
       added bibliographic records that match the search criteria. Thus, a user
       can obtain a custom feed for a particular area of interest simply by
       entering keywords to search and/or selecting filters.
     - Feeds are provided in the [Atom syndication format][Atom].
     - Basic metadata is provided directly in the feeds, using both Atom and
       unqualified [Dublin Core][Dublin_Core] elements.
     - An age limit may be configured to exclude older items from the feeds. This
       may be useful to bibliographies that are frequently updated and mostly
       meant to promote recent literature (all resources still remain visible to
       the search interface regardless of their age).
-- Sitemap: an [XML Sitemap][XML_Sitemap] is automatically generated, and you may
-  use it to help search engines discover your bibliographic records.
-- Exporting: users may export individual records as well as complete
+- **Sitemap**: an [XML Sitemap][XML_Sitemap] is automatically generated, and you
+  may use it to help search engines discover your bibliographic records.
+- **Exporting**: users may export individual records as well as complete
   bibliographies corresponding to search results. By default, download links are
   provided for the RIS and BibTeX formats, but applications may be configured to
   export [any format supported by the Zotero API][Zotero_export].
-- Printing: stylesheets are provided for printing individual bibliographic
+- **Printing**: stylesheets are provided for printing individual bibliographic
   records as well as lists of search results. When printing search results, all
   results get printed (not just the current page of results).
-- Notes and attachments: notes, attached files, and attached links to URIs are
-  synchronized from zotero.org and made available to users of the bibliography.
-  Regular expressions may be used to include or exclude such child items from
-  the bibliography, based on their tags.
-- DOI, ISBN and ISSN resolver: items that have such identifier in your library
-  can be referenced by appending their identifier to your Kerko site's base URL.
-- Relations: bibliographic record pages show links to related items, if any. You
-  may define such relations using Zotero's _Related_ field. Moreover, Kerko adds
-  the _Cites_ and _Cited by_ relation types, which can be managed in Zotero
-  through notes (see [Kerko Recipes](#kerko-recipes). Custom applications
-  can add more types of relations if desired.
-- Badges: icons can be displayed next to items, based on custom conditions.
-- Integration: although a [standalone application][KerkoApp] is available, Kerko
-  itself is not an application, but it can be integrated into any Flask
-  application.
-- Command line interface: Kerko provides commands for synchronizing or deleting
-  its data. These can be invoked through the `flask` command (see [Command line
-  interface](#command-line-interface-cli)).
-
-## Requirements
-
-Kerko requires Python 3.7 or later.
-
-The following Python packages will be automatically installed when installing
-Kerko:
-
-- [Babel]: utilities for internationalization and localization.
-- [Bootstrap-Flask]: helper for integrating [Bootstrap].
-- [Click]: command line interface creation kit.
-- [Flask]: web application framework.
-- [Flask-Babel]: helps Kerko provide its own translations, at the blueprint level.
-- [Flask-WTF]: simple integration of Flask and WTForms.
-- [Jinja2]: template engine.
-- [Pyzotero]: Python client for the Zotero API.
-- [w3lib]: URL and HTML manipulation utilities.
-- [Werkzeug]: WSGI web application library (also required by Flask).
-- [Whoosh]: pure Python full-text indexing and searching library.
-- [WTForms]: web forms validation and rendering library.
-
-The following front-end resources are loaded from CDNs by Kerko's default
-templates (but could be completely removed or replaced by your application):
-
-- [Bootstrap]: front-end component library for web applications.
-- [FontAwesome]: beautiful open source icons.
-- [jQuery]: JavaScript library (required by Bootstrap).
-- [Popper.js]: JavaScript library for handling tooltips, popovers, etc. (used by Bootstrap).
-
-
-## Getting started
-
-This section should help you understand the minimal steps required for getting
-Kerko to work within a Flask application. For a ready-to-use standalone
-application, please refer to [KerkoApp's installation instructions][KerkoApp]
-instead.
-
-Some familiarity with [Flask] should help you make more sense of the
-instructions, but should not be absolutely necessary for getting them to work.
-Let's now build a minimal app, which we'll call `hello_kerko.py`:
-
-1. The first step is to install Kerko. As with any Python library, it is highly
-   recommended to install Kerko within a [virtual environment][venv].
-
-   Once the virtual environment is set and active, use the following command:
-
-   ```bash
-   pip install kerko
-   ```
-
-2. In `hello_kerko.py`, configure variables required by Kerko and create your
-   `app` object, as in the example below:
-
-   ```python
-   import pathlib
-
-   from flask import Flask
-   from kerko.composer import Composer
-
-   app = Flask(__name__)
-   app.config['SECRET_KEY'] = '_5#y2L"F4Q8z\n\xec]/'  # Replace this value.
-   app.config['KERKO_ZOTERO_API_KEY'] = 'xxxxxxxxxxxxxxxxxxxxxxxx'  # Replace this value.
-   app.config['KERKO_ZOTERO_LIBRARY_ID'] = '9999999'  # Replace this value.
-   app.config['KERKO_ZOTERO_LIBRARY_TYPE'] = 'group'  # Replace this value if necessary.
-   app.config['KERKO_DATA_DIR'] = str(pathlib.Path(__file__).parent / 'data' / 'kerko')
-   app.config['KERKO_COMPOSER'] = Composer()
-   ```
-
-   - `SECRET_KEY`: This variable is required for generating secure tokens in web
-     forms. It should have a secure, random value and it really has to be
-     secret. It is usually set in an environment variable rather than in Python
-     code, to make sure it never ends up in a code repository. But here we're
-     taking the minimal route and thus are cutting some corners!
-   - `KERKO_ZOTERO_API_KEY`, `KERKO_ZOTERO_LIBRARY_ID` and
-     `KERKO_ZOTERO_LIBRARY_TYPE`: These variables are required for Kerko to be
-     able to access your Zotero library. See [Configuration
-     variables](#configuration-variables) for details on how to properly set
-     these variables.
-   - `KERKO_DATA_DIR`: This variable specifies the directory where to store the
-     search index and the file attachments. If the specified directory does not
-     already exists, Kerko will try to create it.
-   - `KERKO_COMPOSER`: This variable specifies key elements needed by Kerko,
-     e.g., fields for display and search, facets for filtering. These are
-     defined by instantiating the `Composer` class. Your application may
-     manipulate the resulting object at configuration time to add, remove or
-     alter fields, facets, sort options, search scopes, record download formats,
-     or badges. See [Kerko Recipes](#kerko-recipes) for some examples.
-
-3. Also configure the Flask-Babel and Bootstrap-Flask extensions:
-
-   ```python
-   from flask_babel import Babel
-   from flask_bootstrap import Bootstrap
-
-   babel = Babel(app)
-   bootstrap = Bootstrap(app)
-   ```
-
-   See the respective docs of [Flask-Babel][Flask-Babel_documentation] and
-   [Bootstrap-Flask][Bootstrap-Flask_documentation] for more details.
-
-4. Instantiate the Kerko blueprint and register it in your app:
-
-   ```python
-   from kerko import blueprint as kerko_blueprint
-
-   app.register_blueprint(kerko_blueprint, url_prefix='/bibliography')
-   ```
-
-   The `url_prefix` argument defines the base path for every URL provided by
-   Kerko.
-
-5. In the same directory as `hello_kerko.py` with your virtual environment
-   active, run the following shell commands:
-
-   ```bash
-   export FLASK_APP=hello_kerko.py
-   flask kerko sync
-   ```
-
-   Kerko will retrieve your bibliographic data from zotero.org. If you have a
-   large bibliography or large attachments, this may take a while (and there is
-   no progress indicator). In production use, that command is usually added to
-   the crontab file for regular execution (with enough time between executions
-   for each to complete before the next one starts).
-
-   To list all commands provided by Kerko:
-
-   ```bash
-   flask kerko --help
-   ```
-
-6. Run your application:
-
-   ```bash
-   flask run
-   ```
-
-7. Open http://127.0.0.1:5000/bibliography/ in your browser and explore the
-   bibliography.
-
-You have just built a really minimal application for Kerko. This code example is
-available at [KerkoStart]. However, if you are looking at developing a custom
-Kerko application, we recommend that you consider [KerkoApp] as a starting
-point. While KerkoApp is still quite small, it adds some features and is more
-production-ready than the above example.
-
-
-## Configuration variables
-
-The variables below are required and have no default values:
-
-- `KERKO_COMPOSER`: An instance of the `kerko.composer.Composer` class.
-- `KERKO_DATA_DIR`: The directory where to store the search index and the file
-  attachments. Subdirectories `index` and `attachments` will be created if they
-  do not already exist.
-- `KERKO_ZOTERO_API_KEY`: Your API key, as [created on
-  zotero.org](https://www.zotero.org/settings/keys/new).
-- `KERKO_ZOTERO_LIBRARY_ID`: The identifier of the library to get data from. For
-  your personal library this value should be your _userID_, as found on
-  https://www.zotero.org/settings/keys (you must be logged-in). For a group
-  library this value should be the _groupID_ of the library, as found in the URL
-  of that library (e.g., in https://www.zotero.org/groups/2348869/kerko_demo,
-  the _groupID_ is `2348869`).
-- `KERKO_ZOTERO_LIBRARY_TYPE`: The type of library to get data from, either
-  `'user'` for your personal library, or `'group'` for a group library.
-
-Any of the following variables may be added to your configuration if you wish to
-override their default value:
-
-- `KERKO_CSL_STYLE`: The citation style to use for formatted references. Can be
-  either the file name (without the `.csl` extension) of one of the styles in the
-  [Zotero Styles Repository][Zotero_styles] (e.g., `apa`) or the URL of a remote
-  CSL file. Defaults to `'apa'`.
-- `KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW`: Open attachments in new windows, i.e.,
-  add the `target="_blank"` attribute to attachment links. Defaults to `False`.
-- `KERKO_DOWNLOAD_CITATIONS_LINK`: Provide a record download button on search
-  results pages. Defaults to `True`.
-- `KERKO_DOWNLOAD_CITATIONS_MAX_COUNT`: Limit over which the record download
-  button should be hidden from search results pages. Defaults to `0` (i.e. no
-  limit).
-- `KERKO_FEEDS`: A list of syndication feed formats to publish. Defaults to
-  `['atom']`. If set to an empty list, no web feed will be provided. The only
-  supported format is `'atom'`.
-- `KERKO_FEEDS_FIELDS`: List of fields to retrieve for each feed item (these may
-  be used by the `KERKO_TEMPLATE_ATOM_FEED` template). Values in this list are
-  keys identifying fields defined in the `kerko.composer.Composer` instance. One
-  probably only needs to change the default list when overriding the template to
-  display additional fields. Note that some fields from the default list may be
-  required by other Kerko functions.
-- `KERKO_FEEDS_MAX_DAYS`: The age (in number of days) of the oldest items
-  allowed into web feeds. The Date field of the items are used for that purpose,
-  and when no date is available, the date the item was added to Zotero is used
-  instead. Defaults to `0` (no age limit). Unless your goal is to promote recent
-  literature only, you should probably ignore this setting. Note: Items with
-  missing dates will be considered as very recent, to prevent them from being
-  excluded from feeds. For the same reason, items whose date lack the month
-  and/or the day will be considered as from the 12th month of the year and/or
-  the last day of the month.
-- `KERKO_FULLTEXT_SEARCH`: Allow full-text search of PDF attachments. Defaults
-  to `True`. To get consistent results, see [Ensuring full-text indexing of your
-  attachments in
-  Zotero](#ensuring-full-text-indexing-of-your-attachments-in-zotero).
-- `KERKO_HIGHWIREPRESS_TAGS`: Embed [Highwire Press
-  tags](https://scholar.google.ca/intl/en/scholar/inclusion.html#indexing) into
-  the HTML of item pages. This should help search engines such as Google Scholar
-  index your items, but works only with book, conference paper, journal article,
-  report or thesis items. Defaults to `True` (i.e. enabled).
-- `KERKO_PAGE_LEN`: The number of search results per page. Defaults to `20`.
-- `KERKO_PAGER_LINKS`: Number of pages to show in the pager (not counting the
-  current page). Defaults to `4`.
-- `KERKO_PRINT_ITEM_LINK`: Provide a print button on item pages. Defaults to
-  `False`.
-- `KERKO_PRINT_CITATIONS_LINK`: Provide a print button on search results
-  pages. Defaults to `False`.
-- `KERKO_PRINT_CITATIONS_MAX_COUNT`: Limit over which the print button should
-  be hidden from search results pages. Defaults to `0` (i.e. no limit).
-- `KERKO_RELATIONS_INITIAL_LIMIT`: Number of related items to show above the
-  "show more" link. Defaults to `5`.
-- `KERKO_RELATIONS_LINKS`: Show item links in lists of related items. Defaults
-  to `False`. Enabling this only has an effect if at least one of the following
-  variables is also set to `True`: `KERKO_RESULTS_ATTACHMENT_LINKS`,
-  `KERKO_RESULTS_URL_LINKS`).
-- `KERKO_RESULTS_ABSTRACTS`: Show abstracts on search result pages. Defaults to
-  `False` (abstracts are hidden).
-- `KERKO_RESULTS_ABSTRACTS_TOGGLER`: Show a button letting users show or hide
-  abstracts on search results pages. Defaults to `True` (toggle is displayed).
-- `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH`: Truncate abstracts at the given length
-  (in number of characters). If text is to be truncated in the middle of a word,
-  the whole word is discarded instead. Truncated text is appended with an
-  ellipsis sign ("..."). Defaults to `0` (abstracts get displayed in their full
-  length, without any truncation).
-- `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH_LEEWAY`: If the length of an abstract only
-  exceeds `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH` by this tolerance margin or less
-  (in number of characters), it will not be truncated. Defaults to `0` (no
-  tolerance margin).
-- `KERKO_RESULTS_ATTACHMENT_LINKS`: Provide links to attachments in search
-  results. Defaults to `True`.
-- `KERKO_RESULTS_URL_LINKS`: Provide links to online resources in search
-  results (for items whose URL field has a value). Defaults to `True`.
-- `KERKO_RESULTS_FIELDS`: List of item fields to retrieve for search results
-  (most notably used by the `KERKO_TEMPLATE_SEARCH_ITEM` template). Values in
-  this list are keys identifying fields defined in the `kerko.composer.Composer`
-  instance. One probably only needs to change the default list when overriding
-  the template to display additional fields. Note that some fields from the
-  default list may be required by other Kerko functions.
-- `KERKO_TEMPLATE_SEARCH`: Name of the Jinja2 template to render for the search
-  page with list of results. Defaults to `kerko/search.html.jinja2`.
-- `KERKO_TEMPLATE_SEARCH_ITEM`: Name of the Jinja2 template to render for the
-  search page with a single bibliographic record. Defaults to
-  `kerko/search-item.html.jinja2`.
-- `KERKO_TEMPLATE_ITEM`: Name of the Jinja2 template to render for the
-  bibliographic record view. Defaults to `kerko/item.html.jinja2`.
-- `KERKO_TEMPLATE_ATOM_FEED`: Name of the Jinja2 template used to render an Atom
-  feed. Defaults to `kerko/atom.xml.jinja2`.
-- `KERKO_TEMPLATE_LAYOUT`: Name of the Jinja2 template that is extended by the
-  search, search-item, and item templates. Defaults to `kerko/layout.html.jinja2`.
-- `KERKO_TEMPLATE_BASE`: Name of the Jinja2 template that is extended by the
-  layout template. Defaults to `kerko/base.html.jinja2`.
-- `KERKO_TITLE`: The title to display in web pages. Defaults to `'Kerko'`.
-- `KERKO_ZOTERO_BATCH_SIZE`: Number of items to request on each call to the
-  Zotero API. Defaults to `100` (which is the maximum currently allowed by the
-  API).
-- `KERKO_ZOTERO_MAX_ATTEMPTS`: Maximum number of tries after the Zotero API
-  has returned an error or not responded during indexing. Defaults to `10`.
-- `KERKO_ZOTERO_WAIT`: Time to wait (in seconds) between failed attempts to
-  call the Zotero API. Defaults to `120`.
-- Localization-related variables:
-  - `BABEL_DEFAULT_LOCALE`: The default language of the user interface. Defaults
-    to `'en'`. Your application may set this variable and/or implement a locale
-    selector function to override it (see the [Flask-Babel
-    documentation][Flask-Babel_documentation]).
-  - `BABEL_DEFAULT_TIMEZONE`: The timezone to use for user facing dates.
-    Defaults to `'UTC'`. Your application may set this variable and/or implement
-    a timezone selector function to override it (see the [Flask-Babel
-    documentation][Flask-Babel_documentation]). Any timezone name supported by
-    the [pytz] package should work.
-  - `KERKO_USE_TRANSLATIONS`: Use translations provided by the Kerko package.
-    Defaults to `True`. When this is set to `False`, translations may be
-    provided by the application's own translation catalog.
-  - `KERKO_WHOOSH_LANGUAGE`: The language of search requests. Defaults to
-    `'en'`. You may refer to Whoosh's source to get the list of supported
-    languages (`whoosh.lang.languages`) and the list of languages that support
-    stemming (`whoosh.lang.has_stemmer()`).
-  - `KERKO_ZOTERO_LOCALE`: The locale to use with Zotero API calls. This
-    dictates the locale of Zotero item types, field names, creator types and
-    citations. Defaults to `'en-US'`. Supported locales are listed at
-    https://api.zotero.org/schema, under "locales".
-- `GOOGLE_ANALYTICS_ID`: A Google Analytics property ID, e.g., 'UA-99999-9'.
-  This variable is optional and there is no default value. If set, the Google
-  Analytics tag is inserted into the pages.
-
-**Caution:** Many of the configuration variables cause changes to the structure
-of Kerko's cache or search index. Changing those variables may require that you
-rebuild the cache or the search index, and restart the application. See the
-[command line interface](#command-line-interface-cli) for the cleaning and
-synchronization commands.
-
-
-## Synchronization process
-
-Kerko does one-way data synchronization from zotero.org through a 3-step
-process:
-
-1. Synchronize the Zotero library into a local cache.
-2. Update of the search index from the cache.
-3. Download the file attachments from Zotero.
-
-The first step performs incremental updates of the local cache. After an initial
-full update, the subsequent synchronization runs will request only new and
-updated items from Zotero. This greatly reduces the number of Zotero API calls,
-and thus the time required to complete the synchronization process.
-
-The second step reads data from the cache to update the search index. If the
-cache has changed since the last update, it performs a full update of the search
-index, otherwise it skips to the next step. Any changes to the search index are
-"committed" as a whole at the end of this step, thus up to that point any user
-using the application sees the data that was available prior to the
-synchronization run.
-
-The third and last step reads the list of file attachments from the search
-index, with their MD5 hashes. It compares those with the available local copies
-of the files, and downloads new or changed files from Zotero. It also deletes
-any local files that may no longer be used.
-
-Normally, all synchronization steps are executed. But under certain
-circumstances it can be useful to execute a given step individually. For
-example, after changing some configuration settings, one may clean just the
-search index and rebuild it from the cache (see [the command line
-interface](#command-line-interface-cli) below), which will be much faster than
-re-synchronizing from Zotero.
-
-
-## Command line interface (CLI)
-
-Kerko provides an integration with the [Flask command line interface][Flask_CLI].
-The `flask` command will work with your virtual environment active, and with the
-`FLASK_APP` environment variable set to tell it where to find your application.
+- **Notes and attachments**: notes, attached files, and attached links to URIs
+  are synchronized from zotero.org and made available to users of the
+  bibliography. Regular expressions may be used to include or exclude such child
+  items from the bibliography, based on their tags.
+- **DOI, ISBN and ISSN resolver**: items that have such identifier in your
+  library can be referenced by appending their identifier to your Kerko site's
+  base URL.
+- **Relations**: bibliographic record pages show links to related items, if any.
+  You may define such relations using Zotero's _Related_ field. Moreover, Kerko
+  adds the _Cites_ and _Cited by_ relation types, which can be managed in Zotero
+  through notes. Custom applications can add more types of relations if desired.
+- **Badges**: custom applications can have icons conditionally displayed next to
+  items.
+- **Responsive design**: the simple default implementation works on large
+  monitors as well as on small screens. It is based on [Bootstrap].
+- **Integration**: as a Flask [blueprint][Flask_blueprint], Kerko can be
+  integrated into any Flask application. For a standalone application, however,
+  you may simply install [KerkoApp].
+- **Customizable front-end**: applications may partly or fully replace the
+  default templates, scripts and stylesheets with their own.
+- **Command line interface (CLI)**: Kerko provides commands for synchronizing or
+  deleting its data.
+
+[KerkoApp] is a standalone application built around Kerko. It inherits all of
+Kerko's features and it provides a few additions of its own:
+
+- **Configuration files**: allow separation of configuration from code and
+  enable the [Twelve-factor App][Twelve-factor_App] methodology. Environment
+  variables and [TOML] configuration files are supported. Secrets,
+  server-specific parameters, and general parameters can be configured in
+  separate files.
+- Page templates for common HTTP errors.
+- Syslog logging handler (for Unix environments).
 
-Some frequently used commands are:
 
-```bash
-# List all commands provided by Kerko:
-flask kerko --help
+## Learn more
 
-# Delete all of Kerko's data: cache, search index, attachments.
-flask kerko clean
+Please refer to the [documentation][Kerko_documentation] for more details.
 
-# Get help about the clean command:
-flask kerko clean --help
 
-# Synchronize everything: the cache (from Zotero), the search index (from the
-# cache), the attachments (from files in Zotero, based on list in search index).
-flask kerko sync
-
-# Get help about the sync command:
-flask kerko sync --help
-
-# Delete the cache. A subsequent 'flask kerko sync' will perform a full update
-# from Zotero, but it will not re-download all file attachments.
-flask kerko clean cache
+[Atom]: https://en.wikipedia.org/wiki/Atom_(web_standard)
+[BM25F]: https://en.wikipedia.org/wiki/Okapi_BM25
+[Bootstrap]: https://getbootstrap.com/
+[CSL]: https://citationstyles.org/
+[COinS]: https://en.wikipedia.org/wiki/COinS
+[COinS_clients]: https://en.wikipedia.org/wiki/COinS#Client_tools
+[Dublin_Core]: https://en.wikipedia.org/wiki/Dublin_Core
+[Flask]: https://pypi.org/project/Flask/
+[Flask_blueprint]: https://flask.palletsprojects.com/en/latest/blueprints/
+[Kerko]: https://github.com/whiskyechobravo/kerko
+[Kerko_actions]: https://github.com/whiskyechobravo/kerko/actions
+[Kerko_documentation]: https://whiskyechobravo.github.io/kerko/
+[Kerko_pypi]: https://pypi.org/project/Kerko/
+[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/master/src/kerko/translations
+[KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
+[KerkoApp_demo]: https://demo.kerko.whiskyechobravo.com
+[Snowball]: https://snowballstem.org/
+[TOML]: https://toml.io/
+[Twelve-factor_App]: https://12factor.net/config
+[Whoosh]: https://pypi.org/project/Whoosh/
+[XML_Sitemap]: https://www.sitemaps.org/
+[Zotero]: https://www.zotero.org/
+[Zotero_Connector]: https://www.zotero.org/download/connectors
+[Zotero_demo]: https://www.zotero.org/groups/2348869/kerko_demo/items
+[Zotero_export]: https://www.zotero.org/support/dev/web_api/v3/basics#export_formats
+[Zotero_schema]: https://api.zotero.org/schema
+[Zotero_styles]: https://www.zotero.org/styles/
 
-# Delete just the search index.
-flask kerko clean index
+# Changelog
 
-# Synchronize just the search index (from the cache).
-flask kerko sync index
-```
+For changes that might be specific to KerkoApp, please refer to the [KerkoApp
+changelog](https://github.com/whiskyechobravo/kerkoapp/blob/master/CHANGELOG.md).
 
 
-## Known limitations
+## 1.0.0alpha0
 
-- The system can probably handle relatively large bibliographies (it has been
-  tested so far with ~15k entries), but the number of distinct facet values has
-  more impact on response times. For the best response times, it is recommended
-  to limit the number of distinct facet values to a few hundreds.
-- Kerko can only manage a single bibliography per application.
-- Although Kerko can be integrated in a multilingual web application were the
-  visitor may select a language, Zotero does not provide a way to manage tags or
-  collections in multiple languages. Thus, there is no easy way for Kerko to
-  provide those names in the user's language.
-- Whoosh does not provide much out-of-the-box support for non-Western languages.
-  Therefore, search might not work very well with such languages.
-- Zotero is the sole reference management tool supported as a back-end to Kerko.
-
-
-## Design choices
-
-- Do not build a back-end. Let Zotero act as the "content management" system.
-- Allow Kerko to integrate into richer web applications.
-- Only implement in Kerko features that are related to the exploration of a
-  bibliography. Let other parts of the web application handle all other
-  features that might be needed.
-- Use a lightweight framework (Flask) to avoid carrying many features that are
-  not needed.
-- Use pure Python dependencies to keep installation and deployment simple. Hence
-  the use of Whoosh for search, for example, instead of Elasticsearch or Solr.
-- Use a classic fullstack architecture. Keep it simple and avoid asset
-  management. Some will want to replace the templates and stylesheets anyway.
-
-
-## Kerko Recipes
-
-*TODO: More recipes!*
-
-
-### Ensuring full-text indexing of your attachments in Zotero
-
-Kerko's full-text indexing relies on text content extracted from attachments by
-Zotero. Consequently, for Kerko's full-text search to work, you must make sure
-that full-text indexing works in Zotero first; see [Zotero's documentation on
-full-text
-indexing](https://www.zotero.org/support/searching#pdf_full-text_indexing).
-
-Individual attachments in Zotero can be indexed, partially indexed, or
-unindexed. Various conditions may cause an attachment to be partially indexed or
-unindexed, e.g., file is large, has not been processed yet, or does not contain
-text.
-
-Zotero shows the indexing status in the attachment's right pane. If it shows
-"Indexed: Yes", all is good. If it shows "Indexed: No" or "Indexed: Partial",
-then clicking the "Reindex Item" button (next to the indexing status) should
-ensure that the attachment gets fully indexed, that is if the file actually
-contains text. If there is no "Reindex Item" button, it probably means that
-Zotero does not support that file type for full-text indexing (at the moment, it
-only supports PDF and plain text files).
-
-It can be tedious to go through hundreds of attachments just to find out whether
-they are indexed or not. To make things easier, you could create a [saved
-search](https://www.zotero.org/support/searching#saved_searches) in your Zotero
-library to get an always up-to-date list of unindexed PDFs. Use the following
-search conditions:
-
-- Match *all* of the following:
-    - *Attachment File Type* — *is* — *PDF*
-    - *Attachment Content* — *does not contain* — *.* (that's a period; also
-      select *RegExp* in the small dropdown list, as that will make the period
-      match any character)
-
-This search might return a long list of unindexed attachments. To reindex them
-all at once, you may select them, then right-click to get the contextual menu,
-and select "Reindex items". It may require some time to update your library on
-zotero.org. Note that documents that have no text content, as well as missing
-documents, will still be considered as unindexed and appear in the results of
-the saved search.
-
-Controlling the indexing status will not only improve full-text search on your
-Kerko site, but also full-text search from within Zotero!
-
-
-### Providing _Cites_ and _Cited by_ relations
-
-Zotero allows one to link items together through its _Related_ field. However,
-such relations are not typed nor directed, making it impossible (1) to indicate
-the nature of the relation, or (2) to distinguish which of two related items is
-the citing entity, and which is the one being cited. Consequently, Kerko has its
-own method for setting up those relations.
-
-To establish _Cites_ relations in your Zotero library, you must follow the
-procedure below:
-
-- Install the [Zutilo] plugin for Zotero. Once it is installed, go to _Tools >
-  Zutilo Preferences..._ in Zotero. Then, under _Zotero item menu_, select
-  _Zotero context menu_ next to the _Copy Zotero URIs_ menu item. This
-  configuration step only needs to be done once.
-- Select one or more items from your library that you wish to show as cited by
-  another. Right-click on one of the selected items to open the context menu,
-  and select _Copy Zotero URIs_ from that menu. This copies the references of
-  the selected items items to the clipboard.
-- Right-click the item from your library that cites the items. Select _Add Note_
-  from that item's context menu to add a child note.
-- In the note editor, paste the content of the clipboard. The note should then
-  contain a series of URIs looking like
-  `https://www.zotero.org/groups/9999999/items/ABCDEFGH` or
-  `https://www.zotero.org/users/9999999/items/ABCDEFGH`.
-- At the bottom of the note editor, click into the _Tags_ field and type
-  `_cites`. That tag that will tell Kerko that this particular note is special,
-  that it contains relations.
-
-At the next synchronization, Kerko will retrieve the references found in notes
-tagged with `_cites`. Afterwards, proper hyperlinked citations will appear in
-the _Cites_ and _Cited by_ sections of the related bibliographic records.
-
-Remarks:
-
-- Enter only the _Cites_ relations. The reverse _Cited by_ relations will be
-  inferred automatically.
-- You may only relate items that belong to the same Zotero library.
-- You may use Zotero Item Selects (URIs starting with `zotero://select/`) in the
-  notes, if you prefer those to Zotero URIs.
-- If entered as plain text, URIs must be separated by one or more whitespace
-  character(s). Alternatively, URIs may be entered in HTML links, i.e., in the
-  `href` attribute of `<a>` elements.
-- Hopefully, Zotero will provide nicer ways for handling [relation
-  types](https://sparontologies.github.io/cito/current/cito.html) in the future.
-  In the meantime, using child notes is how Kerko handles it. If relation types
-  are important to you, consider describing your use case in the [Zotero
-  forums](https://forums.zotero.org/discussion/1317/semantic-relations/).
-- Custom Kerko applications can provide more types of relations, if desired, in
-  addition to _Cites_ and _Cited by_.
-
-
-### Submitting your sitemap to search engines
-
-Kerko generates an [XML Sitemap][XML_Sitemap] that can help search engines
-discover your bibliographic records.
-
-The path of the sitemap depends on the configuration of your application. For
-[KerkoApp] or the [Getting started](#getting-started) example above, its path is
-`/bibliography/sitemap.xml`. The full URL of the sitemap then looks like
-`https://example.com/bibliography/sitemap.xml`.
-
-Different search engines may have different procedures for submitting sitemaps
-([Google](https://developers.google.com/search/docs/advanced/sitemaps/build-sitemap#addsitemap),
-[Bing](https://www.bing.com/webmasters/help/Sitemaps-3b5cf6ed),
-[Yandex](https://yandex.com/support/webmaster/indexing-options/sitemap.html)).
-
-However, a standard method consists in adding a `Sitemap` directive to a
-`robots.txt` file served at the root of your site, to tell web crawlers where to
-find your sitemap. For example, you would add the following line to
-`robots.txt`:
+*Warning:* Upgrading from version 0.9 or earlier will require that you adapt
+your installation and configuration (if you are using KerkoApp, make sure to
+check its changelog), then rebuild your search index. Use the following
+commands, then restart the application:
 
+```bash
+flask kerko clean index
+flask kerko sync index
 ```
-Sitemap: https://example.com/bibliography/sitemap.xml
-```
-
-A `robots.txt` file can have multiple `Sitemap` directives, thus the Kerko
-sitemap can be specified alongside any other you might already have.
-
-
-## Translating Kerko
 
-Kerko can be translated using Babel's [setuptools
-integration](http://babel.pocoo.org/en/latest/setup.html).
+Features:
 
-The following commands should be executed from the directory that contains
-`setup.py`, and the appropriate [virtual environment][venv] must have been
-activated beforehand.
+- Add many new configuration parameters. Please refer to the configuration
+  parameters documentation for the full list.
+- Add optional "Open in Zotero" and "View on zotero.org" buttons to item pages.
+  These are disabled by default (see the new settings `KERKO_OPEN_IN_ZOTERO_APP`
+  and `KERKO_OPEN_IN_ZOTERO_WEB`). Even when these settings are enabled, a user
+  who wishes to use such button must first enable it from the (also
+  new) Preferences dialog.
+- Add API for retrieving information about the last synchronization from Zotero.
+- Add the `kerko config` command to the Flask command line interface for
+  displaying all configuration parameters.
+
+Other changes:
+
+- Restructure and expand documentation into a unified documentation site for
+  both Kerko and KerkoApp.
+- Add Portuguese translation. Thanks to Gonçalo Cordeiro.
+
+Backwards incompatible changes:
+
+- Raise the minimum required versions of Flask, Flask-Babel, Bootstrap-Flask,
+  and WTForms. If you have a custom application, some of those may introduce
+  breaking changes.
+- The data directory has a new default location relative to the instance path.
+  Please check the documentation for the `DATA_PATH` and `INSTANCE_PATH`
+  configuration parameters. You may need to set one or both of those parameters,
+  and/or move your existing data directory.
+- Almost all configuration parameters have been renamed and/or moved into a
+  hierarchical structure. Hierarchical parameters are referred to using
+  path-like, dot-separated parameter names, and may conveniently be set with the
+  `kerko.config_helpers.config_set()` function. Here is a mapping of the changed
+  parameters:
+    - `KERKO_BOOTSTRAP_VERSION` → `kerko.assets.bootstrap_version`
+    - `KERKO_CSL_STYLE` → `kerko.zotero.csl_style`
+    - `KERKO_COMPOSER` → `kerko_composer`
+    - `KERKO_DATA_DIR` → `DATA_PATH`. Now optional, relative to the instance
+      path, and defaulting to `kerko` instead of `data/kerko`.
+    - `KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW` → `kerko.features.download_attachment_new_window`
+    - `KERKO_DOWNLOAD_CITATIONS_LINK` → `kerko.features.download_citations_link`
+    - `KERKO_DOWNLOAD_CITATIONS_MAX_COUNT` → `kerko.features.download_citations_max_count`
+    - `KERKO_FEEDS` → `kerko.feeds.formats`
+    - `KERKO_FEEDS_FIELDS` → `kerko.feeds.fields`
+    - `KERKO_FEEDS_MAX_DAYS` → `kerko.feeds.max_days`
+    - `KERKO_FEEDS_REJECT_ANY` → `kerko.feeds.reject_any`
+    - `KERKO_FEEDS_REQUIRE_ANY` → `kerko.feeds.require_any`
+    - `KERKO_FULLTEXT_SEARCH` → `kerko.search.fulltext`
+    - `KERKO_HIGHWIREPRESS_TAGS` → `kerko.meta.highwirepress_tags`
+    - `KERKO_JQUERY_VERSION` → `kerko.assets.jquery_version`
+    - `KERKO_OPEN_IN_ZOTERO_APP` → `kerko.features.open_in_zotero_app`
+    - `KERKO_OPEN_IN_ZOTERO_WEB` → `kerko.features.open_in_zotero_web`
+    - `KERKO_PAGE_LEN` → `kerko.pagination.page_len`
+    - `KERKO_PAGER_LINKS` → `kerko.pagination.pager_links`
+    - `KERKO_POPPER_VERSION` → `kerko.assets.popper_version`
+    - `KERKO_PRINT_CITATIONS_LINK` → `kerko.features.print_citations_link`
+    - `KERKO_PRINT_CITATIONS_MAX_COUNT` → `kerko.features.print_citations_max_count`
+    - `KERKO_PRINT_ITEM_LINK` → `kerko.features.print_item_link`
+    - `KERKO_RELATIONS_INITIAL_LIMIT` → `kerko.features.relations_initial_limit`
+    - `KERKO_RELATIONS_LINKS` → `kerko.features.relations_links`
+    - `KERKO_RELATIONS_SORT` → `kerko.features.relations_sort`
+    - `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH` → `kerko.features.results_abstracts_max_length`
+    - `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH_LEEWAY` → `kerko.features.results_abstracts_max_length_leeway`
+    - `KERKO_RESULTS_ABSTRACTS` → `kerko.features.results_abstracts`
+    - `KERKO_RESULTS_ABSTRACTS_TOGGLER` → `kerko.features.results_abstracts_toggler`
+    - `KERKO_RESULTS_ATTACHMENT_LINKS` → `kerko.features.results_attachment_links`
+    - `KERKO_RESULTS_FIELDS` → `kerko.search.result_fields`
+    - `KERKO_RESULTS_URL_LINKS` → `kerko.features.results_url_links`
+    - `KERKO_TEMPLATE_ATOM_FEED` → `kerko.templates.atom_feed`
+    - `KERKO_TEMPLATE_BASE` → `kerko.templates.base`
+    - `KERKO_TEMPLATE_ITEM` → `kerko.templates.item`
+    - `KERKO_TEMPLATE_LAYOUT` → `kerko.templates.layout`
+    - `KERKO_TEMPLATE_SEARCH` → `kerko.templates.search`
+    - `KERKO_TEMPLATE_SEARCH_ITEM` → `kerko.templates.search_item`
+    - `KERKO_TITLE` → `kerko.meta.title`
+    - `KERKO_WHOOSH_LANGUAGE` → `kerko.search.whoosh_language`
+    - `KERKO_WITH_JQUERY` → `kerko.assets.with_jquery`
+    - `KERKO_WITH_POPPER` → `kerko.assets.with_popper`
+    - `KERKO_ZOTERO_API_KEY` → `ZOTERO_API_KEY`
+    - `KERKO_ZOTERO_BATCH_SIZE` → `kerko.zotero.batch_size`
+    - `KERKO_ZOTERO_LIBRARY_ID` → `ZOTERO_LIBRARY_ID`
+    - `KERKO_ZOTERO_LIBRARY_TYPE` → `ZOTERO_LIBRARY_TYPE`
+    - `KERKO_ZOTERO_LOCALE` → `kerko.zotero.locale`
+    - `KERKO_ZOTERO_MAX_ATTEMPTS` → `kerko.zotero.max_attempts`
+    - `KERKO_ZOTERO_WAIT` → `kerko.zotero.wait`
+- `Composer.__init__()` now only takes a configuration object as argument
+  instead of a bunch of arguments. Thus, the initial values of the `Composer`
+  instance now depend solely on the configuration.
+- Remove the `KERKO_USE_TRANSLATIONS` configuration variable. Kerko now relies
+  on the application's default Babel domain and translation directories. Custom
+  applications that wish to load Kerko's translations should now add
+  `kerko.TRANSLATION_DOMAIN` and `kerko.TRANSLATION_DIRECTORIES` to their Babel
+  configuration.
+- The `__init__()` method of `FacetSpec` and its subclasses now only accept
+  keyword arguments.
+- The `sort_key` argument to `FacetSpec.__init__()` is now `sort_by`.
+- `Composer` built-in fields `z_dateAdded` and `z_dateModified` are now named
+  `date_added` and `date_modified` respectively.
 
-Create or update the PO template (POT) file:
 
-```bash
-python setup.py extract_messages
-```
+## 0.9 (2022-12-29)
 
-Create a new PO file (for a new locale) based on the POT file. Replace
-`YOUR_LOCALE` with the appropriate language code, e.g., `de`, `es`, `fr`:
+*Warning:* Upgrading from version 0.8.x or earlier will require that you rebuild
+your search index. Use the following commands, then restart the application:
 
 ```bash
-python setup.py init_catalog --locale YOUR_LOCALE
+flask kerko clean index
+flask kerko sync index
 ```
 
-Update an existing PO file based on the POT file:
+Features:
 
-```bash
-python setup.py update_catalog --locale YOUR_LOCALE
-```
-
-Compile MO files:
+- Add expand/collapse actions on facet values, allowing full exploration of
+  hierarchical facets without changing the current search.
+- Add an optional initial limit on the number of values to show under each
+  facet. When the initial limit is reached, a "show more" button allows the user
+  to expand the full list.
+- Add Atom syndication feeds.
+- Allow searching items by their Zotero key.
+- Add XML sitemap.
+- Add the `kerko count` CLI command (mostly meant for development purposes).
+
+Bug fixes:
+
+- Fix last sync time not displayed at the bottom of search results when
+  `KERKO_PRINT_CITATIONS_LINK` and `KERKO_DOWNLOAD_CITATIONS_LINK` are both set
+  to `False`.
+- Fix the `kerko sync` CLI command not returning an error code with some types
+  of failures.
+- Fix invalid HTML in help modal.
+
+Other changes:
+
+- Handle new Zotero fields introduced with the new 'preprint' item type.
+- Apply a boost factor to DOI, ISBN and ISSN fields extracted from the Extra
+  field (previously, only the dedicated Zotero fields had a boost factor).
+- Under each facet, always show the facet's active filters first.
+- Make facet values with long labels easier to read (by indenting wrapped lines
+  to the right of the checkbox).
+- Add link to full bibliography from item pages.
+- Add blocks in templates to facilitate theming.
+- Remove `page` parameter from pagination links when `page=1`.
+- Improve documentation.
+- Make sync and schema-related error messages more helpful and user-friendly.
+- Move pydocstyle config to `pyproject.toml`.
+- Tag package as compatible with Python 3.10 and 3.11.
+- Remove leftover code related to Python versions older than 3.7
+
+Backwards incompatible changes:
+
+- Remove the `KERKO_FACET_COLLAPSING` option. The new initial limit on facets
+  values made this feature largely redundant.
+- Remove the `collapsible` param from the `FacetSpec` class.
+- Remove support for configuration variables `KERKO_ZOTERO_START` and
+  `KERKO_ZOTERO_END` (were only used for development and no longer practical).
+
+Changes that might break custom themes:
+
+- The HTML markup and CSS styles of expand/collapse buttons have changed.
+- The parameters of the `facet`, `facet_item`, `facet_items`, `facet_fields`
+  template macros have changed.
+- The `facets-container`, `facets`, and `facets-modal-body` element ids are now
+  required in `search.html.jinja2`.
+
+Possibly backwards incompatible changes (more or less internal API changes):
+
+- Rewrote the `criteria` module. `Criteria.keywords` and `Criteria.filters` work
+  pretty much as before, but everything else has changed.
+- Rewrote the `query` module, which had organically grown into an tangled mess,
+  now replaced with the `searcher` module. This new API is completely different.
+- Adapted view code to the above-mentioned `searcher` API.
+- Split the monolithic `views` module into multiple modules under `views`
+  (`item_creators`, `item_facets`, `item_relations`, `routes`, `search`), and
+  moved `breadbox`, `meta` (as `item_meta`), `pager`, and `sorter` under
+  `views`.
+
+
+## 0.8.1 (2021-11-16)
+
+Bug fixes:
+
+- Fix missing dependency for package building.
+
+
+## 0.8 (2021-11-16)
+
+*Warning:* Upgrading from version 0.7.x or earlier will require that you clean
+and re-sync your existing search index. Use the following commands, then restart
+the application:
 
 ```bash
-python setup.py compile_catalog
+flask kerko clean index
+flask kerko sync
 ```
 
-You are welcome to contribute your translation. See [Submitting a
-translation](#submitting-a-translation).
-
-
-## Contributing
-
-### Reporting issues
+Features:
 
-Issues may be submitted on [Kerko's issue tracker][Kerko_issues]. Please
-consider the following guidelines:
-
-- Make sure that the same issue has not already been reported or fixed in the
-  repository.
-- Describe what you expected to happen.
-- If possible, include a minimal reproducible example to help others identify
-  the issue.
-- Describe what actually happened. Include the full traceback if there was an
-  exception.
-
-
-### Making code changes
-
-Clone the [Kerko repository][Kerko] into a local directory. Set up a [virtual
-environment][venv], then install this local version of Kerko in the virtual
-environment, including development and testing dependencies by running the
-following command from Kerko's root directory, i.e., where `setup.cfg` resides:
-
-```bash
-pip install -e .[dev,tests]
-```
+- Allow full-text search of PDF attachments. This can be disabled by setting
+  `KERKO_FULLTEXT_SEARCH` to `False`. Since this feature relies on Zotero's
+  full-text indexing, you must make sure that it works in Zotero first; see
+  [Zotero's
+  documentation](https://www.zotero.org/support/searching#pdf_full-text_indexing).
+- Add new search scopes "Everywhere" (to search both metadata fields and the
+  text content of attached documents) and "In documents" (to search the text
+  content of attached documents). The scope "In all fields" allows to search all
+  metadata fields, but not the text content of attached documents.
+- Display "View on {hostname}" links under search result items, for quick access
+  to the items' URLs. These can be disabled by setting `KERKO_RESULTS_URL_LINKS`
+  to `False`.
+- Move the "Read" buttons under search result items, as "Read document" links.
+  These can now be disabled by setting `KERKO_RESULTS_ATTACHMENT_LINKS` to
+  `False`.
+- Display DOI field values as hyperlinks (both in DOI fields, and in the Extra
+  field when lines are prefixed with 'DOI:').
+- Add support for imported file attachments, e.g., PDF files imported in your
+  Zotero library through the Zotero Connector. Previously, only "attached copies
+  of files" were supported.
+- Standalone notes and file attachments are now allowed into the search index.
+  Kerko filters them out of search results, but custom applications could search
+  them. A new view, `standalone_attachment_download`, lets one retrieve a
+  standalone file attachment.
+- Add configuration options for truncating long abstracts in search results
+  (`KERKO_RESULTS_ABSTRACTS_MAX_LENGTH` and
+  `KERKO_RESULTS_ABSTRACTS_MAX_LENGTH_LEEWAY`).
+- Embed Highwire Press tags in item pages. This is enabled by default but can be
+  disabled by setting `KERKO_HIGHWIREPRESS_TAGS` to `False`.
+- Allow tracking with Google Analytics (optional).
+- Allow relations in child notes to be specified as HTML links, i.e., in the
+  `href` attribute of `<a>` elements.
+- Allow inclusion or exclusion of items based on multiple tags (previously, only
+  a single pattern could be checked).
 
+Bug fixes:
 
-### Running the tests
+- Fix irrelevant sync warnings, from extractors running on attachment items.
+- Fix empty prev/next links in search pages metadata.
 
-To run basic tests in your current environment:
+Other changes:
+
+- Make synchronization from Zotero much more efficient through incremental
+  updates. Instead of performing a full synchronization each time, Kerko now
+  retrieves just the newly added or updated items. This dramatically reduces the
+  number of Zotero API calls (and time) required to update Kerko's search index.
+  Note: **More work is planned** to eliminate some Zotero API calls that Kerko
+  still makes early in the synchronization process and that could be avoided
+  when its cache is already up-to-date.
+- Add a `sync cache` command to the command line interface.
+- On narrow screens, stack search form controls for better usability.
+- Respond with an HTTP 503 (Service Unavailable) when the search index is empty
+  or unreadable.
+- Make sorts more efficient by setting the `sortable` Whoosh flag on relevant
+  fields.
+- Leading and trailing underscore characters (`_`) are now trimmed from facet
+  value labels. This happens _after_ sorting the values, which means that the
+  underscore can still be used as a prefix to alter the alphabetical order.
+- Support more timezone names. Timezone names such as 'US/Eastern' or
+  'Europe/London' previously did not work, and times could not be converted
+  to daylight saving times.
+- Change labels:
+    - "Print this citation" → "Print this record" (on item pages)
+    - "Download this citation" → "Download this record" (on item & search pages)
+- Inject blocks in item Jinja2 template to facilitate theming.
+- Slightly increase some top/bottom margins.
+- Add the `type` HTML attribute to record download links.
+- Add the `rel="alternate"` HTML attribute to record download links on item
+  pages. Also add a corresponding `link` element to the page `head`.
+- Added utilities for running automated integration tests. This will allow
+  testing many areas of Kerko that previously could hardly be tested.
+
+Backwards incompatible changes:
+
+- Remove deprecated `kerko index` CLI command (use `kerko sync` instead).
+
+Possibly backwards incompatible changes (more or less internal API changes):
+
+- Upgrade many dependencies, including new major versions of Flask (2.x), Jinja2
+  (3.x), Werkzeug (2.x), Click (8.x).
+- The default list for the `KERKO_RESULTS_FIELDS` setting now includes the
+  `'url'` field. If you have overridden that setting in your application and
+  `KERKO_RESULTS_URL_LINKS` is enabled, you'll probably have to add `'url'` too.
+- The schema field `item_type` has been renamed to `item_type_label`. If you
+  have custom templates, please review any use of `item.item_type`.
+- The structure of the `kerko/_search-result.html.jinja2` template has changed
+  somewhat. If you have overridden it, you'll need to review the changes.
+- The `ItemContext` class has been eliminated. The `Extractor.extract()` method
+  now receives an item's dictionary instead of an `ItemContext` object, and if
+  an item has children these are now available directly in the item (with the
+  `children` key). If you have created custom extractor classes, their
+  `extract()` method will need to be adapted accordingly.
+- Some extractor classes have been renamed:
+    - `BaseAttachmentsExtractor` → `BaseChildAttachmentsExtractor`
+    - `BaseNotesExtractor` → `BaseChildNotesExtractor`
+    - `LinkedURIAttachmentsExtractor` → `ChildLinkedURIAttachmentsExtractor`
+    - `NotesTextExtractor` → `ChildNotesTextExtractor`
+    - `RawNotesExtractor` → `RawChildNotesExtractor`
+    - `RelationsInNotesExtractor` → `RelationsInChildNotesExtractor`
+    - `StoredFileAttachmentsExtractor` → `ChildFileAttachmentsExtractor`
+- A view has been renamed:
+    - `item_attachment_download` → `child_attachment_download`
+- A default field has been renamed:
+    - `alternateId` → `alternate_id`
+
+## 0.7.1 (2021-02-04)
+
+Security fixes:
+
+- Fix unescaped date fields, causing a vulnerability to XSS attacks. This
+  vulnerability was introduced in version 0.7.
+
+Bug fixes:
+
+- Fix wrong locale separator in the HTML lang attribute.
+
+Other changes:
+
+- Remove unwanted spacing after dropdown labels.
+
+Documentation changes:
+
+- Fix missing info about library groupID in configuration docs. Thanks
+  [@drmikeuk](https://github.com/drmikeuk) for reporting the issue.
+
+## 0.7 (2021-01-08)
+
+*Warning:* Upgrading from version 0.6 or earlier will require that you clean and
+re-sync your existing search index. Use the following commands, then restart the
+application:
 
 ```bash
-python -m unittest
+flask kerko clean index
+flask kerko sync
 ```
 
-To check code coverage as well, use these commands instead:
+Features:
 
-```bash
-coverage run -m unittest
-coverage report
-```
+- Allow users to toggle the display of abstracts on search results pages.
+- Allow inclusion or exclusion of items based on their tags
+  ([#4](https://github.com/whiskyechobravo/kerko/issues/4)).
+- Show attached links to URIs on item pages.
+- Show relations on item pages. The relation types provided by default are:
+  - _Related_, based on Zotero's _Related_ field.
+  - _Cites_, managed through child notes containing Zotero URIs and tagged with
+    the `_cites` tag.
+  - _Cited by_, automatically inferred from _Cites_ relations.
+- The Extra field is now searched when searching "in any fields".
+- Items that have a DOI, ISBN or ISSN identifier can be referenced by appending
+  their identifier to your Kerko site's base URL.
+- Requests for the older URL of an item whose ID has changed are now
+  automatically redirected to the item's current URL. This relies on the
+  `dc.replaces` relation that's managed internally by Zotero on some operations
+  such as item merges.
+- Help users who might mistakenly bookmark a search result's URL rather than the
+  item's permanent URL: Add an `id` parameter to the search result URLs, and
+  redirect the user to that item's permanent URL if the search result no longer
+  matches because of database changes.
+- Redirect to the parent item's page when the user tries to request an
+  attachment that no longer exists.
+- Improve accessibility based on WCAG recommendations and WAI-ARIA standards:
+  - Add labels to search form elements.
+  - Add landmark role `search` to the search form.
+  - Make the purpose of various links more obvious through improved or added
+    labels.
+  - Add the `aria-label` attribute to many elements.
+  - Add text to indicate the current value of widgets.
+  - Add the `aria-current` attribute to indicate the current value of widgets.
+  - Remove useless link to the current page from the pagination widget.
+
+Bug fixes:
+
+- Fix crash when trying to sync a link attachment
+  ([#3](https://github.com/whiskyechobravo/kerko/issues/3)).
+- Fix unhandled exception during sync when an attachment cannot be downloaded.
+- Fix page numbers greater than the page count in search URLs generating wrong
+  page numbers for search result item URLs.
+- Fix secondary keys getting sorted in reverse order with some sort options,
+  e.g., when sorting by newest first, results having the same date were then
+  sorted by creator name in reverse alphabetical order instead of alphabetical
+  order.
+- Fix empty HTML element taking up horizontal space when there are no badges.
+
+Other changes:
+
+- Display ISO 8601 calendar dates in a more readable format, using the
+  formatting style of the locale.
+- Show a timezone abbreviation along with time of last update from Zotero.
+- Add German translation. Thanks to [@mmoole](https://github.com/mmoole).
+- Fix broken "Getting started" example in README.
+- Migrate most package distribution options and metadata from `setup.py` to
+  `setup.cfg`.
+- Migrate project to a `src` layout.
+- Use Flask-Babel instead of its fork Flask-BabelEx, now that is has merged the
+  translation domain features from Flask-BabelEx.
+
+Backwards incompatible changes:
+
+- Drop support for Python 3.6. Kerko is no longer being tested under Python 3.6.
+  Known issue with 3.6 at this point: some ISO 8601 dates cannot be parsed and
+  reformatted; instead of being displayed in a locale-sensitive manner, these
+  get displayed as is. More issues might arise in the future with Python 3.6 as
+  Kerko continues to evolve.
+- All values of the `pager` dict passed to the `_pager.html.jinja2` template are
+  now lists. Previously, only the values at keys `'before'` and `'after'` were
+  lists; now the values at keys `'previous'`, `'first'`, `'current'`, `'last'`,
+  and `'next'` are lists as well.
+- The words `'blacklist'` and `'whitelist'` in variable names are replaced with
+  `'exclude'` and `'include'`.
+- The `KERKO_RESULTS_ABSTRACT` configuration variable is replaced by two
+  variables, `KERKO_RESULTS_ABSTRACTS` (note the now plural form) and
+  `KERKO_RESULTS_ABSTRACTS_TOGGLER`.
+- Citation download URLs now have the form
+  `{url_prefix}/{itemID}/export/{format}` for individual items (`'export'` has
+  been inserted), and `{url_prefix}/export/{format}/` for search result pages
+  (`'download'` has been replaced by `'export'`).
+- The `Extractor` class' interface has changed, improving consistency and
+  separation of concerns:
+  - All arguments to `__init__()` must now be specified as keyword arguments.
+  - The `extract()` method no longer have a `document` argument, and the `spec`
+    argument is now the last one. The method now returns a value instead of
+    assigning it to the document.
+  - The new `extract_and_store()` method handles extraction, encoding, and
+    assignment to the document, assigning the value only when it is not `None`.
+- The `AttachmentsExtractor` class has been renamed to
+  `StoredFileAttachmentsExtractor`.
+- `InCollectionExtractor` now extends collection membership to subcollections.
+  To preserve the previous behavior, set the `check_subcollections` parameter to
+  `False` when initializing the extractor.
+
+Possibly backwards incompatible changes (more or less internal API changes):
+
+- The `search_results` variable passed to the `search.html.jinja2` template is
+  now an iterator of tuples, where the first element of each tuple is a result,
+  and the second element the URL of the result.
+
+## 0.6 (2020-06-15)
+
+Security fixes:
+
+- Fix multiple vulnerabilities to XSS attacks. **All previous versions of Kerko
+  were vulnerable, thus an upgrade is highly recommended.**
+
+Backwards incompatible changes:
+
+- Remove default value for the `KERKO_DATA_DIR` configuration variable. KerkoApp
+  users don't need to worry about this as KerkoApp takes care of it, but custom
+  apps that did not already set this variable now have to.
+
+Features:
+
+- Open PDF documents in the browser's built-in PDF viewer (instead of opening
+  the browser's file download popup).
+- Add buttons for opening documents directly from search result pages (these
+  replace the previous paperclip badges).
+- Add button at the top of item pages for opening documents (makes the
+  availability of such documents much more obvious).
+- Add the `KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW` configuration variable to
+  control whether to open documents in a new window or in the same window.
+- Display the date and time of the last successful synchronization from Zotero
+  at the bottom of search results.
+
+Bug fixes:
+
+- Preserve newlines when displaying the value of the Extra field.
+- Preserve newlines when displaying abstracts in search result pages.
+- Fix filters missing on search pages that have no results.
+- Avoid empty box in print media when there is no search criteria.
+- Avoid empty box when the search index is missing.
+- Fix pluralization in CLI time elapsed messages.
+
+Other changes:
+
+- Refer to attachments as "documents" in the interface, and replace the
+  paperclip icon with a file icon.
+- Remove CSRF token from search form. Token expiration can impede legitimate
+  users, and the token is unnecessary as the form does not change the
+  application's state.
+- Add a proper message when none of the filters provided in the URL are
+  recognized.
+- Improve documentation.
+- Add INFO-level log message to report successful synchronization from Zotero.
+- Add blocks in templates to facilitate theming.
+
+Possibly backwards incompatible changes (more or less internal API changes):
+
+- Rename the `content_with_badges` template macro as `badges`, and leave it to
+  the caller to display content.
+- Remove badges that are related to attachments.
 
-Note: Test coverage is still very low at the moment. You are welcome to
-contribute new tests!
+## 0.5 (2019-11-19)
 
-To run the full test suite under different environments (using the various
-Python interpreters available on your machine):
+*Warning:* Upgrading from version 0.4 or earlier will require that you clean and
+re-sync your existing search index. Use the following commands:
 
 ```bash
-tox
+flask kerko clean index
+flask kerko sync
 ```
 
+Features:
 
-### Submitting code changes
-
-Pull requests may be submitted against [Kerko's repository][Kerko]. Please
-consider the following guidelines:
-
-- Before submitting, run the tests and make sure they pass. Add tests relevant
-  to your change (those should fail if ran without your patch).
-- Use [Yapf](https://github.com/google/yapf) to autoformat your code (with
-  option `--style='{based_on_style: facebook, column_limit: 100}'`). Many
-  editors provide Yapf integration.
-- Include a string like "Fixes #123" in your commit message (where 123 is the
-  issue you fixed). See [Closing issues using
-  keywords](https://help.github.com/en/articles/closing-issues-using-keywords).
-- If a Jinja2 template represents a page fragment or a collection of macros,
-  prefix its file name with the underscore character.
-
-
-### Submitting a translation
-
-Some guidelines:
-
-- The PO file encoding must be UTF-8.
-- The header of the PO file must be filled out appropriately.
-- All messages of the PO file must be translated.
-
-Please submit your translation as a pull request against [Kerko's
-repository][Kerko], or by [e-mail][Kerko_email], with the PO file included as an
-attachment (**do not** copy the PO file's content into an e-mail's body, since
-that could introduce formatting or encoding issues).
-
-
-### Supporting the project
-
-Nurturing an open source project such as Kerko, following up on issues and
-helping others in working with the system is a lot of work, but hiring the
-original developers of Kerko can do a lot in ensuring continued support and
-development of the project.
-
-If you need professional support related to Kerko, have requirements not
-currently implemented in Kerko, want to make sure that some Kerko issue
-important to you gets resolved, or if you just like our work and would like to
-hire us for an unrelated project, please [e-mail us][Kerko_email].
-
-
-## Changelog
-
-For a summary of changes by release version, see the [changelog](CHANGELOG.md).
-
-
-## Project background
-
-Kerko was inspired by two prior projects:
-
-- [Bibliographie sur l’histoire de
-  Montréal](https://bibliomontreal.uqam.ca/bibliographie/), developed in 2014 by
-  David Lesieur and Patrick Fournier, of Whisky Echo Bravo, for the [Laboratoire
-  d'histoire et de patrimoine de Montréal](https://lhpm.uqam.ca/) (Université du
-  Québec à Montréal, Canada).
-- [Bibliography on English-speaking Quebec](http://quescren.concordia.ca/),
-  developed in 2017 by David Lesieur, for the [Quebec English-Speaking
-  Communities Research Network
-  (QUESCREN)](https://www.concordia.ca/artsci/scpa/quescren.html) (Concordia
-  University, Canada).
+- Add support for Zotero attachments.
+- Allow configuration of badges on items. The 'attachment' badge is provided by
+  default, displaying an icon on items that have one or more attachments.
+- Add help modal.
+- Improve customizability:
+  - Add `KERKO_TEMPLATE_*` configuration variables for page template names.
+  - Use configurable, separate templates to render facets and badges (see the
+    `renderer` argument to `kerko.specs.FacetSpec`, `kerko.specs.BadgeSpec`).
+  - Add the `KERKO_RESULTS_FIELDS` configuration variable to specify which
+    fields to retrieve with search queries.
+- Add building blocks for creating boolean facets based on collection membership
+  (new class `kerko.extractors.InCollectionExtractor`, new parameters for
+  `kerko.codecs.BooleanFacetCodec`).
+
+Bug fixes:
+
+- Fix facets not ordered by weight on item page.
+- Preserve newlines in abstract display.
+- Fix incorrect use of bookmark link on item pages, set canonical link instead.
+- Prevent text overflow in some browsers on citations containing long URLs.
+
+Other changes:
+
+- Deprecate CLI command `kerko index` in favor of new command `kerko sync`.
+- Change title of the "Refine" panel to "Explore".
+- Change labels of the "Print" and "Download" buttons to "Print this citation"
+  and "Download this citation", to prevent any confusion with attachment
+  downloading.
+- Show the facets in a more robust and accessible Bootstrap modal, on small
+  screens, instead of the home-built drawer.
+- Use compact pagination widget on small screens.
+- Tweak sizing, positioning, and spacing of various UI elements.
+- Improve accessibility of various UI elements.
+- Make citation stand out more in item page.
+- Hide some elements and decorations in print media.
+- Make search query more efficient on item page.
+
+Possibly backwards incompatible changes (more or less internal API changes):
+
+- Force keyword arguments with `kerko.composer.Composer.__init__()`.
+- Rename `kerko.composer.Composer.__init__()` arguments
+  `default_note_whitelist_re` as `default_child_whitelist_re`,
+  `default_note_blacklist_re` as `default_child_blacklist_re`.
+- Rename method `kerko.views.item()` as `kerko.views.item_view()`.
+- Rename template file `_facet.html.jinja2` as `_facets.html.jinja2`.
+- Replace argument `checkboxes` in template macro `field()` with `add_link_icon`
+  and `remove_link_icon`.
+
+## 0.4 (2019-09-28)
+
+Features:
+
+- Allow search term boosting in relevance score calculation, e.g. `faceted^2
+  search browsing^0.5`.
+
+Security fixes:
+
+- Update minimum Werkzeug version to 0.15.3. See
+  [CVE-2019-14806](https://nvd.nist.gov/vuln/detail/CVE-2019-14806): "Pallets
+  Werkzeug before 0.15.3, when used with Docker, has insufficient debugger PIN
+  randomness because Docker containers share the same machine id."
+
+Other changes:
+
+- Update jQuery version to 3.4.1.
+- Update French translations (translate boolean search operators).
+- Improve search form validation and error display.
+- Disable not-so-intuitive boolean search operators (`AndNot`, `AndMaybe`,
+  `Require` were unwanted but enabled by default by Whoosh's `OperatorsPlugin`).
+- Improve documentation.
+- Code cleanup.
 
-Later on, it became clear that other organizations needed a similar solution.
-However, software from the prior projects had to be rewritten so it could more
-easily be configured for different bibliographies from organizations with
-different needs. That led to Kerko, whose development was made possible through
-the following project:
+## 0.3 (2019-07-29)
 
-- [Bibliographie francophone sur l'archivistique](https://bibliopiaf.ebsi.umontreal.ca/),
-  funded by the
-  [Association internationale des archives francophones (AIAF)](http://www.aiaf.org/)
-  and hosted by the
-  [École de bibliothéconomie et des sciences de l’information (EBSI)](https://ebsi.umontreal.ca/)
-  (Université de Montréal, Canada).
+Features:
 
+- Exporting: users may export individual citations as well as complete
+  bibliographies corresponding to search results. By default, download links are
+  provided for the RIS and BibTeX formats, but applications may be configured to
+  export any format supported by the Zotero API.
 
-### Etymology
+Bug fixes:
 
-The name _Zotero_ reportedly derives from the Albanian word _zotëroj_, which
-means "to learn something extremely well, that is to master or acquire a skill
-in learning" (Source: Mark Dingemanse, 2008, [Etymology of
-Zotero](http://ideophone.org/zotero-etymology/)).
+- Fix bad alignment of field names in print mode.
+- Remove warning when indexing an item with no authors
+  ([#1](https://github.com/whiskyechobravo/kerko/issues/1)).
 
-The name _Kerko_ is a nod to Zotero as it takes a similar etymological route: it
-derives from the Albanian word _kërkoj_, which means "to ask, to request, to
-seek, to look for, to demand, to search" and seems fit to describe a search
-tool.
+Other changes:
 
+- Move print button to bottom of search pages (next to the new download
+  dropdown).
+- Improve documentation.
+- Compile message catalog before building sdist and wheel.
 
-## Powered by Kerko
+Possibly backwards incompatible changes (more or less internal API changes):
 
-The following online bibliographies are powered by Kerko:
+- Method `kerko.composer.Composer.get_ordered_specs()` replaces
+  `get_ordered_scopes()`, `get_ordered_facets()` and `get_ordered_sorts()`.
 
-- [Bibliographie francophone sur l'archivistique](https://bibliopiaf.ebsi.umontreal.ca/)
-- [Community Knowledge Open Library on English-Speaking Quebec](https://ckol.quescren.ca/)
-- [Lipedema Foundation LEGATO Lipedema Library](https://library.lipedema.org/)
-- [Open Development & Education Evidence Library](https://docs.opendeved.net/)
-- [The EdTech Hub Evidence Library](http://docs.edtechhub.org/)
-- [University of Saint Joseph Research Output](https://research.usj.edu.mo/)
+## 0.3alpha1 (2019-07-17)
 
-If you wish to add your Kerko-powered online bibliography to this list, please
-[e-mail us][Kerko_email] or submit a pull request.
+- Fix broken links in documentation.
 
+## 0.3alpha0 (2019-07-16)
 
-[Atom]: https://en.wikipedia.org/wiki/Atom_(web_standard)
-[Babel]: https://pypi.org/project/Babel/
-[BM25F]: https://en.wikipedia.org/wiki/Okapi_BM25
-[Bootstrap]: https://getbootstrap.com/
-[Bootstrap-Flask]: https://pypi.org/project/Bootstrap-Flask/
-[Bootstrap-Flask_documentation]: https://bootstrap-flask.readthedocs.io/en/latest/basic.html
-[Click]: https://pypi.org/project/click/
-[COinS]: https://en.wikipedia.org/wiki/COinS
-[COinS_clients]: https://en.wikipedia.org/wiki/COinS#Client_tools
-[CSL]: https://citationstyles.org/
-[Dublin_Core]: https://en.wikipedia.org/wiki/Dublin_Core
-[Flask]: https://pypi.org/project/Flask/
-[Flask_blueprint]: https://flask.palletsprojects.com/en/latest/blueprints/
-[Flask-Babel]: https://pypi.org/project/Flask-Babel/
-[Flask-Babel_documentation]: https://flask-babel.tkte.ch/
-[Flask_CLI]: https://flask.palletsprojects.com/en/latest/cli/
-[Flask-WTF]: https://pypi.org/project/Flask-WTF/
-[FontAwesome]: https://fontawesome.com/icons
-[HighwirePress_Google]: https://scholar.google.ca/intl/en/scholar/inclusion.html#indexing
-[Jinja2]: https://pypi.org/project/Jinja2/
-[jQuery]: https://jquery.com/
-[Kerko]: https://github.com/whiskyechobravo/kerko
-[Kerko_actions]: https://github.com/whiskyechobravo/kerko/actions
-[Kerko_email]: mailto:kerko@whiskyechobravo.com
-[Kerko_issues]: https://github.com/whiskyechobravo/kerko/issues
-[Kerko_pypi]: https://pypi.org/project/Kerko/
-[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/master/kerko/translations
-[KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
-[KerkoApp_demo]: https://demo.kerko.whiskyechobravo.com
-[KerkoStart]: https://github.com/whiskyechobravo/kerkostart
-[Popper.js]: https://popper.js.org/
-[Python]: https://www.python.org/
-[pytz]: https://pypi.org/project/pytz/
-[Pyzotero]: https://pypi.org/project/Pyzotero/
-[Snowball]: https://snowballstem.org/
-[venv]: https://docs.python.org/3.8/tutorial/venv.html
-[w3lib]: https://pypi.org/project/w3lib/
-[Werkzeug]: https://pypi.org/project/Werkzeug/
-[Whisky_Echo_Bravo]: https://whiskyechobravo.com
-[Whoosh]: https://pypi.org/project/Whoosh/
-[WTForms]: https://pypi.org/project/WTForms/
-[XML_Sitemap]: https://www.sitemaps.org/
-[Zotero]: https://www.zotero.org/
-[Zotero_Connector]: https://www.zotero.org/download/connectors
-[Zotero_demo]: https://www.zotero.org/groups/2348869/kerko_demo/items
-[Zotero_export]: https://www.zotero.org/support/dev/web_api/v3/basics#export_formats
-[Zotero_schema]: https://api.zotero.org/schema
-[Zotero_styles]: https://www.zotero.org/styles/
-[Zotero_web_api]: https://www.zotero.org/support/dev/web_api/start
-[Zutilo]: https://github.com/willsALMANJ/Zutilo
+- First PyPI release.
```

### Comparing `Kerko-0.9/pyproject.toml` & `Kerko-1.0.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/setup.cfg` & `Kerko-1.0.0a0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = Kerko
-version = 0.9
+version = 1.0.0alpha0
 author = David Lesieur
 author_email = kerko@whiskyechobravo.com
 license_files = LICENSE.txt
 url = https://github.com/whiskyechobravo/kerko
 project_urls = 
-	Documentation = https://github.com/whiskyechobravo/kerko
+	Documentation = https://whiskyechobravo.github.io/kerko/
 	Code = https://github.com/whiskyechobravo/kerko
 	Changes = https://github.com/whiskyechobravo/kerko/blob/master/CHANGELOG.md
 	Issue tracker = https://github.com/whiskyechobravo/kerko/issues
 description = A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 keywords = academia, bibliography, bibliographies, flask, search, zotero
@@ -31,57 +31,67 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Database :: Front-Ends
 	Topic :: Education
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Internet :: WWW/HTTP :: Indexing/Search
+	Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 	Topic :: Scientific/Engineering
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find_namespace:
 package_dir = =src
 python_requires = >=3.7
 install_requires = 
 	Babel >=2.6.0
-	Bootstrap-Flask >=1.0.10, <2.0
+	Bootstrap-Flask >=2.0.1
 	click >=8.0.1
-	Flask >=2.0.1, <2.3
-	Flask-Babel >=2.0.0
+	dpath >=2.1.0
+	Flask >=2.2.5
+	Flask-Babel >=3.0.1
 	Flask-WTF >=0.14.2
-	Jinja2 >=3.0.1, <3.1
+	Jinja2 >=3.0.1
+	pydantic >=1.10.7, <2.0
+	python-dotenv >=0.21.1
+	pytz  # Babel does not require it (since 2.12.0), but will use it if present.
 	Pyzotero >=1.4.26
+	tomli >=2.0.1
 	w3lib >=1.22.0
 	Werkzeug >=2.0.1
 	Whoosh >=2.7.4
 	wrapt >=1.10.0
-	WTForms >=2.2, <3.0
+	WTForms >=3.0.0
 include_package_data = True
 setup_requires = 
 	Babel >=2.6.0  # For compiling catalog.
 	wheel >=0.38.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 tests = 
-	coverage >=6.1.2, <6.4
-	elementpath >=2.4.0, <3
+	coverage >=6.1.2, <8
+	elementpath >=2.4.0, <5
 	lxml >=4.6.4, <5
-	responses >=0.15.0, <0.18
-	tox >=3.8, <4
+	responses >=0.17.0
+	tox >=3.8, <5
 dev = 
+	mypy >=0.910
 	pip-tools >=5.5.0
 	pycodestyle
 	pydocstyle >=6.1.0
 	pylint >=2.5.0
 	rope
 	yapf
+docs = 
+	mkdocs-material >=9.1.15
+	mike >=1.1.2
 
 [options.entry_points]
 flask.commands = 
 	kerko = kerko.cli:cli
 
 [aliases]
 dist = sdist bdist_wheel
@@ -118,11 +128,14 @@
 domain = kerko
 statistics = 1
 
 [yapf]
 based_on_style = facebook
 column_limit = 100
 
+[mypy]
+plugins = pydantic.mypy
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `Kerko-0.9/setup.py` & `Kerko-1.0.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/Kerko.egg-info/SOURCES.txt` & `Kerko-1.0.0a0/src/Kerko.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 babel.cfg
+mkdocs.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+docs/background.md
+docs/changelog.md
+docs/config-basics.md
+docs/config-params.md
+docs/contributing.md
+docs/deployment.md
+docs/getting-started.md
+docs/index.md
+docs/localization.md
+docs/recipes.md
+docs/synchronization.md
+docs/troubleshooting.md
 src/Kerko.egg-info/PKG-INFO
 src/Kerko.egg-info/SOURCES.txt
 src/Kerko.egg-info/dependency_links.txt
 src/Kerko.egg-info/entry_points.txt
 src/Kerko.egg-info/requires.txt
 src/Kerko.egg-info/top_level.txt
 src/kerko/__init__.py
 src/kerko/cli.py
 src/kerko/codecs.py
 src/kerko/composer.py
+src/kerko/config_helpers.py
 src/kerko/criteria.py
 src/kerko/datetime.py
+src/kerko/default_config.toml
 src/kerko/exceptions.py
 src/kerko/extractors.py
 src/kerko/forms.py
 src/kerko/jinja2.py
 src/kerko/renderers.py
 src/kerko/searcher.py
 src/kerko/shortcuts.py
@@ -30,14 +45,15 @@
 src/kerko/storage.py
 src/kerko/tags.py
 src/kerko/text.py
 src/kerko/transformers.py
 src/kerko/tree.py
 src/kerko/static/kerko/css/styles.css
 src/kerko/static/kerko/js/item.js
+src/kerko/static/kerko/js/open_in_zotero.js
 src/kerko/static/kerko/js/print.js
 src/kerko/static/kerko/js/search.js
 src/kerko/sync/__init__.py
 src/kerko/sync/attachments.py
 src/kerko/sync/cache.py
 src/kerko/sync/index.py
 src/kerko/sync/zotero.py
@@ -49,14 +65,15 @@
 src/kerko/templates/kerko/_facet_field.html.jinja2
 src/kerko/templates/kerko/_facet_search.html.jinja2
 src/kerko/templates/kerko/_facets.html.jinja2
 src/kerko/templates/kerko/_item-relations.html.jinja2
 src/kerko/templates/kerko/_navbar_brand.html.jinja2
 src/kerko/templates/kerko/_navbar_items.html.jinja2
 src/kerko/templates/kerko/_pager.html.jinja2
+src/kerko/templates/kerko/_preferences.html.jinja2
 src/kerko/templates/kerko/_search-form.html.jinja2
 src/kerko/templates/kerko/_search-help.html.jinja2
 src/kerko/templates/kerko/_search-metas.html.jinja2
 src/kerko/templates/kerko/_search-result.html.jinja2
 src/kerko/templates/kerko/_sorter.html.jinja2
 src/kerko/templates/kerko/atom.xml.jinja2
 src/kerko/templates/kerko/base.html.jinja2
@@ -66,26 +83,30 @@
 src/kerko/templates/kerko/search.html.jinja2
 src/kerko/templates/kerko/sitemap.xml.jinja2
 src/kerko/templates/kerko/sitemap_index.xml.jinja2
 src/kerko/translations/de/LC_MESSAGES/kerko.mo
 src/kerko/translations/de/LC_MESSAGES/kerko.po
 src/kerko/translations/fr/LC_MESSAGES/kerko.mo
 src/kerko/translations/fr/LC_MESSAGES/kerko.po
+src/kerko/translations/pt/LC_MESSAGES/kerko.mo
+src/kerko/translations/pt/LC_MESSAGES/kerko.po
 src/kerko/views/__init__.py
 src/kerko/views/breadbox.py
-src/kerko/views/item_creators.py
-src/kerko/views/item_facets.py
-src/kerko/views/item_meta.py
-src/kerko/views/item_relations.py
 src/kerko/views/pager.py
 src/kerko/views/routes.py
 src/kerko/views/search.py
 src/kerko/views/sorter.py
+src/kerko/views/item/__init__.py
+src/kerko/views/item/creators.py
+src/kerko/views/item/facets.py
+src/kerko/views/item/meta.py
+src/kerko/views/item/relations.py
 tests/__init__.py
 tests/test_atom_feed.py
+tests/test_config.py
 tests/test_datetime.py
 tests/test_item_meta.py
 tests/test_pager.py
 tests/test_sitemap.py
 tests/test_sync.py
 tests/test_tags.py
 tests/integration_testing/README.md
```

### Comparing `Kerko-0.9/src/kerko/cli.py` & `Kerko-1.0.0a0/src/kerko/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 @click.argument(
     'target',
     type=click.Choice(['cache', 'index'], case_sensitive=False),
 )
 @with_appcontext
 def count(target):
     """
-    Output the number of records available in the cache or in the search index.
+    Show the number of records available in the cache or in the search index.
 
     The cache and the index are structured very differently and their respective
     numbers should not be expected to match. The number of records in the index
     may not even match the number of results obtained in Kerko's search
     interface, because the search can do some internal filtering.
 
     The cache is a flat database where items of any type or hierarchical level
@@ -106,14 +106,23 @@
         pprint.pprint(get_doc_count(target))
     except SearchIndexError as e:
         current_app.logger.error(e)
         raise click.Abort
 
 
 @cli.command()
+@with_appcontext
+def config():
+    """
+    Show the app's full configuration.
+    """
+    pprint.pprint(dict(current_app.config))
+
+
+@cli.command()
 @click.argument('item_key')
 @with_appcontext
 def zotero_item(item_key):
     """
     Retrieve an item from the library, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
```

### Comparing `Kerko-0.9/src/kerko/codecs.py` & `Kerko-1.0.0a0/src/kerko/codecs.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/criteria.py` & `Kerko-1.0.0a0/src/kerko/criteria.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,25 +168,25 @@
 
     def initialize_sort(self, initial):
         sort_spec = composer().sorts.get(initial.get('sort', ''))
         if sort_spec and sort_spec.is_allowed(self):
             self.options['sort'] = sort_spec.key
 
     def initialize_abstracts(self, initial):
-        if config('KERKO_RESULTS_ABSTRACTS_TOGGLER'):
-            enabled_by_default = config('KERKO_RESULTS_ABSTRACTS')
+        if config('kerko.features.results_abstracts_toggler'):
+            enabled_by_default = config('kerko.features.results_abstracts')
             abstracts = initial.get('abstracts')
             if abstracts:
                 if abstracts in ['t', '1'] and not enabled_by_default:
                     self.options['abstracts'] = 1
                 elif abstracts in ['f', '0'] and enabled_by_default:
                     self.options['abstracts'] = 0
 
     def initialize_print_preview(self, initial):
-        if config('KERKO_PRINT_CITATIONS_LINK') and initial.get('print-preview') in [
+        if config('kerko.features.print_citations_link') and initial.get('print-preview') in [
             't', '1'
         ]:
             self.options['print-preview'] = 1
 
     def initialize_id(self, initial):
         if self.options.get('page-len') == 1 and initial.get('id'):
             self.options['id'] = initial.get('id')
```

### Comparing `Kerko-0.9/src/kerko/datetime.py` & `Kerko-1.0.0a0/src/kerko/datetime.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/exceptions.py` & `Kerko-1.0.0a0/src/kerko/exceptions.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/extractors.py` & `Kerko-1.0.0a0/src/kerko/extractors.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import itertools
 import re
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from datetime import datetime
 
-from flask import Markup, current_app
+from flask import current_app
+from markupsafe import Markup
 
 from kerko.datetime import maximize_partial_date, parse_partial_date
 from kerko.tags import TagGate
 from kerko.text import id_normalize, sort_normalize
 from kerko.transformers import (find_item_id_in_zotero_uri_links,
                                 find_item_id_in_zotero_uris_str)
 
@@ -254,14 +255,45 @@
             item_fields = [f for f in fields if f.get('field') in item['data']]
             return item_fields
         if item_type != 'attachment':  # Attachment has no field metadata, no need to warn.
             self.warning(f"Missing or unknown item type '{item_type}'", item)
         return None
 
 
+class ItemLinkExtractor(Extractor):
+    """Extract an item link from the 'links' element."""
+
+    def __init__(self, *, link_key, link_type, **kwargs):
+        super().__init__(**kwargs)
+        self.link_key = link_key
+        self.link_type = link_type
+
+    def extract(self, item, library_context, spec):
+        link = item.get('links', {}).get(self.link_key, {})
+        if link and link.get('type') == self.link_type:
+            return link.get('href')
+        return None
+
+
+class ZoteroWebItemURLExtractor(ItemLinkExtractor):
+    """Extract an item's zotero.org link."""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(link_key='alternate', link_type='text/html', *args, **kwargs)
+
+
+class ZoteroAppItemURLExtractor(Extractor):
+    """Extract a link for opening the item in the Zotero app."""
+
+    def extract(self, item, library_context, spec):
+        if library_context.library_type == 'group':
+            return f"zotero://select/groups/{library_context.library_id}/items/{item.get('key')}"
+        return f"zotero://select/library/items/{item.get('key')}"
+
+
 class CreatorTypesExtractor(Extractor):
     """Extract creator types metadata."""
 
     def extract(self, item, library_context, spec):
         item_type = item.get('data', {}).get('itemType')
         if item_type and item_type in library_context.creator_types:
             library_creator_types = library_context.creator_types[item_type]
```

### Comparing `Kerko-0.9/src/kerko/jinja2.py` & `Kerko-1.0.0a0/src/kerko/jinja2.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 from __future__ import annotations
 
 import re
 import typing
 from urllib.parse import urlparse
 
-from jinja2 import Markup, evalcontextfilter
+from jinja2 import pass_eval_context
+from markupsafe import Markup
 from w3lib.url import safe_url_string
 
 from kerko.datetime import format_datetime, reformat_date
 
 if typing.TYPE_CHECKING:
     from flask.blueprints import BlueprintSetupState
 
 
-@evalcontextfilter
+@pass_eval_context
 def urlize_doi(eval_ctx, doi, target=None, rel=None, link=True):
     """Convert the specified DOI to an URL."""
     if not re.match(r'^https?://', doi, flags=re.IGNORECASE):
         url = 'https://doi.org/' + str(doi)
     else:
         url = str(doi)
     if link:
@@ -31,15 +32,15 @@
     else:
         result = url
     if eval_ctx.autoescape:
         result = Markup(result)
     return result
 
 
-@evalcontextfilter
+@pass_eval_context
 def parse_and_urlize_doi(eval_ctx, text, target=None, rel=None):
     """Convert a DOI to an URL, on all lines having the 'DOI:' prefix."""
     target = f' target="{target}"' if target else ''
     rel = f' rel="{rel}"' if rel else ''
     result = re.sub(
         r'^(?P<prefix>\s*DOI:\s*)(?!https?://)(?P<doi>\S+)\s*$',
         r'\g<prefix><a href="https://doi.org/\g<doi>"' + target + rel + r'>\g<doi></a>',
```

### Comparing `Kerko-0.9/src/kerko/renderers.py` & `Kerko-1.0.0a0/src/kerko/renderers.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/searcher.py` & `Kerko-1.0.0a0/src/kerko/searcher.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/specs.py` & `Kerko-1.0.0a0/src/kerko/specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,22 +122,23 @@
 
 
 class FacetSpec(BaseFieldSpec):
     """Specifies a facet for search grouping and filtering."""
 
     def __init__(
             self,
+            *,
             title,
             filter_key,
             weight=0,
             initial_limit=0,
-            initial_limit_leeway=0,
+            initial_limit_leeway=2,
             codec=None,
             missing_label=None,
-            sort_key=None,
+            sort_by=None,
             sort_reverse=False,
             item_view=True,
             allow_overlap=True,
             query_class=None,
             renderer=None,
             **kwargs
     ):
@@ -185,15 +186,15 @@
         self.title = title
         self.filter_key = filter_key
         self.weight = weight
         self.initial_limit = initial_limit
         self.initial_limit_leeway = initial_limit_leeway
         self.codec = codec or BaseFacetCodec()
         self.missing_label = missing_label
-        self.sort_key = sort_key
+        self.sort_by = sort_by
         self.sort_reverse = sort_reverse
         self.item_view = item_view
         self.allow_overlap = allow_overlap
         self.query_class = query_class or Term
         self.renderer = renderer or renderers.TemplateResolverRenderer(
             'kerko/_facet_{mode}.html.jinja2'
         )
@@ -242,15 +243,15 @@
             facet will be built for performing a new search.
 
         :param active_only: Only build the items that are related to active
             filters, i.e., filters actually present in the search criteria.
         """
 
     def sort_items(self, items):
-        if self.sort_key is None:
+        if self.sort_by is None:
             return
 
         # Sort items based on multiple-keys.
         return sorted(
             items,
             key=lambda x: (
                 # First sort key: show active items first.
@@ -260,15 +261,15 @@
                 # Third sort key: sort items according to the facet's specified
                 # sort keys. If 'count' is used as key, multiply the count value
                 # by -1 to reverse order (because the desired default when
                 # ordering by count is the descending order).
                 *[
                     x[k] * -1 if k == 'count' else
                     (sort_normalize(x[k]) if isinstance(x[k], str) else x[k])
-                    for k in self.sort_key
+                    for k in self.sort_by
                 ]
             ),
             reverse=self.sort_reverse
         )
 
     def render(self, items, mode):
         return self.renderer.render(spec=self, items=items, mode=mode)
@@ -492,21 +493,20 @@
     """
     Specifies a facet based on a top-level Zotero collection.
 
     A top-level Zotero collection can act as a facet when its key matches a
     given `collection_key`. Subcollections become values within the facet.
     """
 
-    def __init__(self, collection_key, **kwargs):
-        # Provide more convenient defaults for this type of facet.
-        kwargs.setdefault('key', 'collection_facet_' + collection_key)
+    def __init__(self, *, collection_key, **kwargs):
+        # Provide some convenient defaults for this type of facet.
+        kwargs.setdefault('key', f'facet_collection_{collection_key}')
         kwargs.setdefault('field_type', ID(stored=True))
-        kwargs.setdefault('filter_key', slugify(kwargs.get('title')))
+        kwargs.setdefault('filter_key', slugify(str(kwargs.get('title'))))
         kwargs.setdefault('codec', CollectionFacetCodec())
-        kwargs.setdefault('sort_key', ['label'])
         kwargs.setdefault('query_class', Prefix)
         kwargs.setdefault('extractor', extractors.CollectionFacetTreeExtractor())
         super().__init__(**kwargs)
         self.collection_key = collection_key
 
 
 class SortSpec:
```

### Comparing `Kerko-0.9/src/kerko/static/kerko/css/styles.css` & `Kerko-1.0.0a0/src/kerko/static/kerko/css/styles.css`

 * *Files 5% similar despite different names*

```diff
@@ -80,7 +80,16 @@
   mask-image: linear-gradient(to top, transparent, black 2.75rem);
 }
 main {
   min-height: calc(100vh - 7rem);
   padding-top: 1rem;
   padding-bottom: 3rem;
 }
+.btn-toggle[active] > .btn-toggle-icon-off {
+  display: none;
+}
+.btn-toggle:not([active]) > .btn-toggle-icon-on {
+  display: none;
+}
+.d-none-important {
+  display: none !important;
+}
```

### Comparing `Kerko-0.9/src/kerko/static/kerko/js/print.js` & `Kerko-1.0.0a0/src/kerko/static/kerko/js/print.js`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/static/kerko/js/search.js` & `Kerko-1.0.0a0/src/kerko/static/kerko/js/search.js`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/storage.py` & `Kerko-1.0.0a0/src/kerko/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pathlib
 import pickle
 import shutil
 
 import whoosh
 
-from kerko.shortcuts import config
+from kerko.shortcuts import data_path
 
 
 class SearchIndexError(Exception):
     pass
 
 
 class SchemaError(Exception):
     pass
 
 
 def get_storage_dir(storage):
-    return pathlib.Path(config('KERKO_DATA_DIR')) / storage
+    return pathlib.Path(data_path()) / storage
 
 
 def load_object(storage, key, default=None):
     try:
         with open(get_storage_dir(storage) / f'{key}.pickle', 'rb') as f:
             return pickle.load(f)
     except IOError:
```

### Comparing `Kerko-0.9/src/kerko/sync/attachments.py` & `Kerko-1.0.0a0/src/kerko/sync/attachments.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import hashlib
 
 from flask import current_app
 
 from kerko.extractors import is_file_attachment
 from kerko.searcher import Searcher
-from kerko.shortcuts import composer
+from kerko.shortcuts import composer, config
 from kerko.storage import get_storage_dir, open_index
 from kerko.sync import zotero
 
 
 def md5_checksum(path):
     # Hash file in 8k blocks to avoid reading it all in memory.
     with path.open('rb') as f:
@@ -66,15 +66,17 @@
     index = open_index('index')
     with Searcher(index) as searcher:
         count = 0
         results = searcher.search(limit=None)  # Retrieve all items.
         for item in results.items(
             composer().select_fields(['id', 'item_type', 'attachments', 'data'])
         ):
-            if item['item_type'] == 'attachment' and is_file_attachment(item, composer().mime_types):
+            if item['item_type'] == 'attachment' and is_file_attachment(
+                item, config('kerko.zotero.attachment_mime_types')
+            ):
                 _sync_attachment(item)
                 count += 1
             else:
                 # Child attachments, unlike standalone attachments (above), do not
                 # need their linkMode or MIME type to be validated, because that has
                 # already been done by an extractor when writing the search index.
                 for attachment in item.get('attachments', []):
```

### Comparing `Kerko-0.9/src/kerko/sync/cache.py` & `Kerko-1.0.0a0/src/kerko/sync/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     library_context = zotero.request_library_context(zotero_credentials)  # TODO: Load pickle & sync collections incrementally
     since = load_object('cache', 'version', default=0)
     version = zotero.last_modified_version(zotero_credentials)
 
     cache = open_index('cache', schema=get_cache_schema, auto_create=True, write=True)
     writer = cache.writer(limitmb=256)
     try:
-        if config('KERKO_FULLTEXT_SEARCH'):
+        if config('kerko.search.fulltext'):
             fulltext_items = zotero.load_new_fulltext(zotero_credentials, since)
         else:
             fulltext_items = {}
 
         formats = get_formats()
         for item in zotero.Items(zotero_credentials, since=since, formats=list(formats) + ['data']):
             count += 1
```

### Comparing `Kerko-0.9/src/kerko/sync/index.py` & `Kerko-1.0.0a0/src/kerko/sync/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Update the search index from the local cache."""
 
 import whoosh
 from flask import current_app
 from whoosh.query import Term
 
-from kerko.shortcuts import composer
+from kerko.shortcuts import composer, config
 from kerko.storage import (SchemaError, SearchIndexError, load_object,
                            open_index, save_object)
 from kerko.tags import TagGate
 
 
 def sync_index():
     """
@@ -41,25 +41,29 @@
         return yield_items(parent['key'])
 
     count = 0
     index = open_index('index', schema=composer().schema, auto_create=True, write=True)
     writer = index.writer(limitmb=256)
     try:
         writer.mergetype = whoosh.writing.CLEAR
-        gate = TagGate(composer().default_item_include_re, composer().default_item_exclude_re)
+        gate = TagGate(
+            config('kerko.zotero.item_include_re'),
+            config('kerko.zotero.item_exclude_re'),
+        )
         for item in yield_top_level_items():
             count += 1
             if gate.check(item['data']):
                 item['children'] = list(yield_children(item))  # Extend the base Zotero item dict.
                 document = {}
                 for spec in list(composer().fields.values()) + list(composer().facets.values()):
                     spec.extract_to_document(document, item, library_context)
                 writer.update_document(**document)
                 current_app.logger.debug(
-                    f"Item {count} updated ({item['key']}, {item.get('itemType')}): {document.get('z_title')}"
+                    f"Item {count} updated ({item['key']}, {item.get('itemType')}): "
+                    f"{document.get('data', {}).get('title')}"
                 )
             else:
                 current_app.logger.debug(f"Item {count} excluded ({item['key']})")
     except (whoosh.fields.FieldConfigurationError, whoosh.fields.UnknownFieldError) as e:
         writer.cancel()
         current_app.logger.error(e)
         raise SchemaError("Schema changes are required. Please clean index.") from e
```

### Comparing `Kerko-0.9/src/kerko/sync/zotero.py` & `Kerko-1.0.0a0/src/kerko/sync/zotero.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,35 @@
             return wrapped(*args, **kwargs)
         except (
                 requests.exceptions.ConnectionError,
                 zotero_errors.HTTPError,
                 zotero_errors.UnsupportedParams
         ) as e:
             current_app.logger.warning(e)
-            if attempts < config('KERKO_ZOTERO_MAX_ATTEMPTS'):
+            if attempts < config('kerko.zotero.max_attempts'):
                 current_app.logger.warning(
                     f"The Zotero API request has failed in {wrapped.__name__}. "
-                    f"New attempt in {config('KERKO_ZOTERO_WAIT')} seconds..."
+                    f"New attempt in {config('kerko.zotero.wait')} seconds..."
                 )
                 attempts += 1
-                sleep(config('KERKO_ZOTERO_WAIT'))
+                sleep(config('kerko.zotero.wait'))
             else:
                 current_app.logger.error(
                     "The maximum number of API call attempts to Zotero has "
                     "been reached. Stopping."
                 )
                 raise
 
 
 def init_zotero():
     return zotero.Zotero(
-        library_id=config('KERKO_ZOTERO_LIBRARY_ID'),
-        library_type=config('KERKO_ZOTERO_LIBRARY_TYPE'),
-        api_key=config('KERKO_ZOTERO_API_KEY'),
-        locale=config('KERKO_ZOTERO_LOCALE')
+        library_id=config('ZOTERO_LIBRARY_ID'),
+        library_type=config('ZOTERO_LIBRARY_TYPE'),
+        api_key=config('ZOTERO_API_KEY'),
+        locale=config('kerko.zotero.locale')
     )
 
 
 def request_library_context(zotero_credentials):
     item_types = {
         t['itemType']: t['localized']
         for t in load_item_types(zotero_credentials)
@@ -230,15 +230,15 @@
         )
         start = 0
         if top_level:
             method = zotero_credentials.collections_top
         else:
             method = zotero_credentials.collections
         while True:
-            more = method(start=start, limit=config('KERKO_ZOTERO_BATCH_SIZE'))
+            more = method(start=start, limit=config('kerko.zotero.batch_size'))
             if not more:
                 break
             start += len(more)
             for collection in more:
                 self.collections[collection['key']] = collection
 
     def __iter__(self):
@@ -328,27 +328,27 @@
             try:
                 return self._next_item()
             except StopIteration:
                 self._next_batch()
 
     @retry_zotero
     def _next_batch(self):
-        limit = config('KERKO_ZOTERO_BATCH_SIZE')
+        limit = config('kerko.zotero.batch_size')
         current_app.logger.info(
             f"Requesting up to {limit} {self.method_info} items since version {self.since}, "
             f"starting at position {self.start}..."
         )
         params = {
             'since': self.since,
             'start': self.start,
             'limit': limit,
             'sort': 'dateAdded',
             'direction': 'asc',
             'include': self.include,
-            'style': config('KERKO_CSL_STYLE'),
+            'style': config('kerko.zotero.csl_style'),
         }
         self.zotero_batch = getattr(self.zotero_credentials, self.method)(**params)
         if not self.zotero_batch:
             raise StopIteration  # Empty batch, nothing more to iterate on.
         self.iterator = iter(self.zotero_batch)
 
     def _next_item(self):
```

### Comparing `Kerko-0.9/src/kerko/tags.py` & `Kerko-1.0.0a0/src/kerko/tags.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_badges.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_badges.html.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% macro badges(item, mode, wrapper_classes='float-right ml-2 py-2') %}
     {%- set badge_ns = namespace(has_active_badges=False) %}
-    {%- for badge in config.KERKO_COMPOSER.get_ordered_specs('badges') %}
+    {%- for badge in config.kerko_composer.get_ordered_specs('badges') %}
         {%- if badge.is_active(item) %}
             {%- set badge_ns.has_active_badges = True %}
         {%- endif %}
     {%- endfor %}
     {%- if badge_ns.has_active_badges %}
         <span class="{{ wrapper_classes }}">
-            {%- for badge in config.KERKO_COMPOSER.get_ordered_specs('badges') %}
+            {%- for badge in config.kerko_composer.get_ordered_specs('badges') %}
                 {{ badge.render(item, mode) }}
             {%- endfor %}
         </span>
     {%- endif %}
 {% endmacro %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_breadbox.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_breadbox.html.jinja2`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {%- from "kerko/_facets.html.jinja2" import facet -%}
 
 {%- if breadbox %}
     {%- if breadbox.keywords %}
-        {%- for scope in config.KERKO_COMPOSER.get_ordered_specs('scopes') %}
+        {%- for scope in config.kerko_composer.get_ordered_specs('scopes') %}
             {{- facet(
                     scope.breadbox_label,
                     '',
                     breadbox.keywords[scope.key],
                     wrap_class='row',
                     heading_tag='div',
                     heading_class='col-md-4 col-xl-3 font-weight-bold break-word text-md-right text-print-left',
@@ -14,15 +14,15 @@
                     list_class_top='list-unstyled mb-0',
                     remove_title=_("Remove the '{}' search term")
                 )
             }}
         {%- endfor %}
     {%- endif %}
     {%- if breadbox.filters %}
-        {%- for f in config.KERKO_COMPOSER.get_ordered_specs('facets') %}
+        {%- for f in config.kerko_composer.get_ordered_specs('facets') %}
             {{ f.render(breadbox.filters[f.key], 'breadbox') }}
         {%- endfor %}
     {%- endif %}
 {%- elif is_searching %}
     <div class="row">
         <div class="col">
             {{ _("None of your search criteria could be recognized.") }}
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {%- from "kerko/_facets.html.jinja2" import facet -%} {%- if breadbox %} {%- if
-breadbox.keywords %} {%- for scope in config.KERKO_COMPOSER.get_ordered_specs
+breadbox.keywords %} {%- for scope in config.kerko_composer.get_ordered_specs
 ('scopes') %} {{- facet( scope.breadbox_label, '', breadbox.keywords
 [scope.key], wrap_class='row', heading_tag='div', heading_class='col-md-4 col-
 xl-3 font-weight-bold break-word text-md-right text-print-left',
 body_class='col-md-8 col-xl-9', list_class_top='list-unstyled mb-0',
 remove_title=_("Remove the '{}' search term") ) }} {%- endfor %} {%- endif %}
-{%- if breadbox.filters %} {%- for f in config.KERKO_COMPOSER.get_ordered_specs
+{%- if breadbox.filters %} {%- for f in config.kerko_composer.get_ordered_specs
 ('facets') %} {{ f.render(breadbox.filters[f.key], 'breadbox') }} {%- endfor %}
 {%- endif %} {%- elif is_searching %}
 {{ _("None of your search criteria could be recognized.") }} {{__("Reset
 search")_}}.
 {%- endif %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_collapse.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_collapse.html.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -10,13 +10,13 @@
             collapse_description='',
             collapse_icon='fas fa-chevron-up',
             icons_width='',
             expand_default=False
         )
     -%}
     <button class="{{ [btn_class, 'btn-expand']|join(' ') }}" data-toggle="collapse" data-target="#{{ collapse_id }}" aria-controls="{{ collapse_id }}" aria-expanded="{% if expand_default %}true{% else %}false{% endif %}" {% if expand_description %}{{ title_aria_label(expand_description) }}{% endif %}>
-        {%- if expand_icon %}<span class="{{ expand_icon }}" aria-hidden="true" {% if icons_width %}style="width: {{ icons_width }};"{% endif %}></span>{% if expand_label %} {{ expand_label }}{% endif %}{% endif -%}
+        {%- if expand_icon %}<span class="{{ expand_icon }}" aria-hidden="true" {% if icons_width %}style="width: {{ icons_width }};"{% endif %}></span>{% endif -%}{% if expand_label %} {{ expand_label }}{% endif %}
     </button>{#- No whitespace -#}
     <button class="{{ [btn_class, 'btn-collapse']|join(' ') }}" data-toggle="collapse" data-target="#{{ collapse_id }}" aria-controls="{{ collapse_id }}" aria-expanded="{% if expand_default %}false{% else %}true{% endif %}" {% if collapse_description %}{{ title_aria_label(collapse_description) }}{% endif %}>
-        {%- if collapse_icon %}<span class="{{ collapse_icon }}" aria-hidden="true" {% if icons_width %}style="width: {{ icons_width }};"{% endif %}></span>{% if collapse_label %} {{ collapse_label }}{% endif %}{% endif -%}
+        {%- if collapse_icon %}<span class="{{ collapse_icon }}" aria-hidden="true" {% if icons_width %}style="width: {{ icons_width }};"{% endif %}></span>{% endif -%}{% if collapse_label %} {{ collapse_label }}{% endif %}
     </button>
 {%- endmacro %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_facet_field.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_field.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_facets.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_facets.html.jinja2`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 {%- macro facet(
             title,
             missing_label,
             items,
             list_id='',
             initial_limit=0,
-            initial_limit_leeway=0,
+            initial_limit_leeway=2,
             wrap_tag='div', wrap_class='',
             heading_tag='h3', heading_class='h6 font-weight-bold',
             body_tag='div', body_class='',
             list_class_top='list-unstyled'
         )
     -%}
     {%- if items %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_pager.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_pager.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_search-form.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-form.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_search-help.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-help.html.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
                     <p>{{ _("You may start searching either from the <strong>{}</strong> section or from the <strong>{}</strong> section.").format(_("Search"), _("Explore")) }}</p>
                     <h3>{{ _("Search") }}</h3>
                     <p>{{ _("This section shows your current search criteria and allows you to submit keywords to search in the bibliography.") }}</p>
                     <ul>
                         <li>{{ _("Each new submission adds the entered keywords to the list of search criteria.") }}</li>
                         <li>{{ _("To start a new search instead of adding keywords to the current search, use the <strong>{}</strong> button, then enter your new keywords.").format(_("Reset search")) }}</li>
                         <li>{{ _("To replace an already submitted keyword, first remove it by unchecking its checkbox, then submit a new keyword.") }}</li>
-                        {%- if config.KERKO_COMPOSER.scopes|length %}
+                        {%- if config.kerko_composer.scopes|length %}
                             <li>{{ _("You may control the extent of your search by selecting where to search. The options are:") }}
                                 <ul>
-                                    {%- for scope in config.KERKO_COMPOSER.scopes.values() %}
+                                    {%- for scope in config.kerko_composer.scopes.values() %}
                                         {%- if scope.help_text %}
                                             <li><strong>{{ scope.selector_label }}</strong>{{ _(": ") }}{{ scope.help_text }}</li>
                                         {%- endif %}
                                     {%- endfor %}
                                 </ul>
                             </li>
                         {%- endif %}
@@ -51,22 +51,22 @@
                     <ul>
                         <li>{{ _("Categories can be used to filter your search. Check a category to add it to your search criteria and narrow your search. Your search results will then only show entries that are associated with that category.") }}</li>
                         <li>{{ _("Uncheck a category to remove it from your search criteria and broaden your search results.") }}</li>
                         <li>{{ _("The numbers shown next to the categories indicate how many entries are associated with each category in the current set of results. Those numbers will vary based on your search criteria to always describe the current set of results. Likewise, categories and whole facets will disappear when the result set has no entry associated to them.") }}</li>
                         <li>{{ _("An arrow icon ({}) appearing next to a category indicates that subcategories are available. You may press it to expand a list of more specific categories. You may press it again later to collapse the list. Expanding or collapsing subcategories will not change your current search; this allows you to quickly explore a hierarchy of categories if desired.").format('<span class="fas fa-chevron-right" aria-hidden="true"></span>') }}</li>
                     </ul>
                     <h3>{{ _("Results") }}</h3>
-                    <p>{{ _("This section shows the search results. When no search criteria has been given, it shows the full content of the bibliography (up to {page_len} entries per page).").format(page_len=config.KERKO_PAGE_LEN) }}</p>
+                    <p>{{ _("This section shows the search results. When no search criteria has been given, it shows the full content of the bibliography (up to {page_len} entries per page).").format(page_len=config.kerko.pagination.page_len) }}</p>
                     <ul>
                         <li>{{ _("Each entry of the results list is a link to its full bibliographic record. From the bibliographic record view, you may continue exploring the search results by going to previous or following records in your search results, or you may return to the list of results.") }}</li>
                         <li>{{ _("Additional links, such as <strong>Read document</strong> or <strong>View on <em>[website name]</em></strong>, may appear under a result. These give you quick access to the resource. Those links will also be available in the full bibliographic record.") }}</li>
-                        {%- if config.KERKO_RESULTS_ABSTRACTS_TOGGLER %}
+                        {%- if config.kerko.features.results_abstracts_toggler %}
                             <li>{{- _("The <strong>Abstracts</strong> button lets you toggle the display of abstracts within the list of search results. Enabling abstracts, however, will have no effect on results for which no abstract is available.") }}
                         {%- endif %}
-                        {%- if config.KERKO_COMPOSER.sorts|length %}
+                        {%- if config.kerko_composer.sorts|length %}
                             <li>{{ _("Various options are provided to let you sort the search results. One of them is the <strong>Relevance</strong> option, which ranks the results from most relevant to least relevant. The score used for ranking takes into account word frequencies as well as the fields where they appear. For instance, if a search term occurs frequently in an entry or is one of very few terms used in that entry, that entry will probably rank higher than another where the search term occurs less frequently or where lots of other words also occur. Likewise, a search term will have more effect on the scores if it is rare in the whole bibliography than if it is very common. Also, if a search term appears in, e.g., the title of an entry, it will have more effect on the score of that entry than if it appeared in a less important field such as the abstract.") }}</li>
                             <li>{{ _("The <strong>Relevance</strong> sort is only available after keywords have been submitted using the <strong>{search}</strong> section.").format(search=_("Search")) }}</li>
                             <li>{{ _("Categories selected in the <strong>{explore}</strong> section have no effect on the relevance score. Their only effect is to filter the list of results.").format(explore=_("Explore")) }}</li>
                         {%- endif %}
                     </ul>
                     <div class="my-3 text-right">
                         <button type="button" class="btn btn-secondary" data-dismiss="modal" aria-label="{{ _('Close Help panel') }}">{{ _("Close") }}</button>
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_search-metas.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-metas.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_search-result.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-result.html.jinja2`

 * *Files 24% similar despite different names*

```diff
@@ -21,50 +21,50 @@
                     {{- result.coins|safe -}}
                 {%- endif %}
             </div>
         {%- endblock search_item_display %}
     {%- endif -%}
     {%- if show_abstracts and result.data['abstractNote']|trim|length %}
         <p class="{% block search_abstract_classes %}search-abstract pre-line pl-3 my-2{% endblock %}">
-            {%- if config.KERKO_RESULTS_ABSTRACTS_MAX_LENGTH > 0 %}
+            {%- if config.kerko.features.results_abstracts_max_length > 0 %}
                 {{- result.data['abstractNote']|truncate(
-                        config.KERKO_RESULTS_ABSTRACTS_MAX_LENGTH,
-                        leeway=config.KERKO_RESULTS_ABSTRACTS_MAX_LENGTH_LEEWAY
+                        config.kerko.features.results_abstracts_max_length,
+                        leeway=config.kerko.features.results_abstracts_max_length_leeway
                     )|escape|urlize(target='_blank')|trim -}}
             {%- else %}
                 {{- result.data['abstractNote']|escape|urlize(target='_blank')|trim -}}
             {%- endif %}
         </p>
     {%- endif %}
     {%- if not hide_result_links %}
         {%- block search_result_links %}
-            {%- if result.attachments|length and config.KERKO_RESULTS_ATTACHMENT_LINKS or result.url|kerko_url_hostname and config.KERKO_RESULTS_URL_LINKS %}
+            {%- if result.attachments|length and config.kerko.features.results_attachment_links or result.url|kerko_url_hostname and config.kerko.features.results_url_links %}
                 <div class="d-print-none btn-group {% block search_item_links_classes %}ml-2{% endblock %}">
-                    {%- if config.KERKO_RESULTS_ATTACHMENT_LINKS and result.attachments|length > 1 %}
+                    {%- if config.kerko.features.results_attachment_links and result.attachments|length > 1 %}
                         {%- block search_result_link_multiple_attachments %}
                             <div class="dropdown">
                                 <button class="{% block search_item_attachments_btn_classes %}btn btn-sm btn-link dropdown-toggle text-nowrap{% endblock %}" type="button" id="attachment-options-{{ result.id|escape }}" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                     <span class="fas fa-file mr-1" aria-hidden="true"></span>{{ _('Read documents') -}}
                                 </button>
                                 <span class="dropdown-menu dropdown-menu-right dropdown-width-300" aria-labelledby="attachment-options-{{ result.id|escape }}">
                                     {%- for attachment in result.attachments %}
-                                        <a class="dropdown-item" href="{{ url_for('kerko.child_attachment_download', item_id=result.id, attachment_id=attachment['id'], attachment_filename=attachment['data']['filename']) }}"{% if config.KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW %} target="_blank"{% endif %}>
+                                        <a class="dropdown-item" href="{{ url_for('kerko.child_attachment_download', item_id=result.id, attachment_id=attachment['id'], attachment_filename=attachment['data']['filename']) }}"{% if config.kerko.features.download_attachment_new_window %} target="_blank"{% endif %}>
                                             {{- attachment['data']['filename']|escape }}
                                         </a>
                                     {%- endfor %}
                                 </span>
                             </div>
                         {%- endblock search_result_link_multiple_attachments %}
-                    {%- elif config.KERKO_RESULTS_ATTACHMENT_LINKS and result.attachments|length == 1 %}
+                    {%- elif config.kerko.features.results_attachment_links and result.attachments|length == 1 %}
                         {%- block search_result_link_single_attachment %}
-                            <a class="{% block search_item_attachment_btn_classes %}btn btn-sm btn-link text-nowrap{% endblock %}" href="{{ url_for('kerko.child_attachment_download', item_id=result.id, attachment_id=result.attachments[0]['id'], attachment_filename=result.attachments[0]['data']['filename']) }}"{% if config.KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW %} target="_blank"{% endif %} {{ title_aria_label(_('Read \'{}\'').format(result.attachments[0]['data']['filename']|escape)) }}>
+                            <a class="{% block search_item_attachment_btn_classes %}btn btn-sm btn-link text-nowrap{% endblock %}" href="{{ url_for('kerko.child_attachment_download', item_id=result.id, attachment_id=result.attachments[0]['id'], attachment_filename=result.attachments[0]['data']['filename']) }}"{% if config.kerko.features.download_attachment_new_window %} target="_blank"{% endif %} {{ title_aria_label(_('Read \'{}\'').format(result.attachments[0]['data']['filename']|escape)) }}>
                                 <span class="fas fa-file mr-1" aria-hidden="true"></span>{{ _('Read document') -}}
                             </a>
                         {%- endblock search_result_link_single_attachment %}
-                    {%- elif config.KERKO_RESULTS_URL_LINKS and result.url|kerko_url_hostname %}
+                    {%- elif config.kerko.features.results_url_links and result.url|kerko_url_hostname %}
                         {%- block search_result_link_url %}
                             <a class="{% block search_item_link_btn_classes %}btn btn-sm btn-link text-nowrap{% endblock %}" href="{{ result.url|kerko_url_sanitize|escape }}" target="_blank">
                                 <span class="fas fa-external-link-alt mr-1" aria-hidden="true"></span>{{ _('View on {}').format(result.url|kerko_url_hostname|escape) -}}
                             </a>
                         {%- endblock search_result_link_url %}
                     {%- endif %}
                 </div>
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/_sorter.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/_sorter.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/templates/kerko/atom.xml.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/atom.xml.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <feed {% block feed_attributes %}xmlns="http://www.w3.org/2005/Atom" xmlns:dc="http://purl.org/dc/elements/1.1/"{% endblock %}>
     {%- block feed_elements %}
         {%- block feed_title %}
-            <title type="html">{{ config.KERKO_TITLE|escape }} - {{ feed_title|escape }}</title>
+            <title type="html">{{ config.kerko.meta.title|escape }} - {{ feed_title|escape }}</title>
         {%- endblock %}
         {%- block feed_author %}
             <author>
-                <name>{{ config.KERKO_TITLE|escape }}</name>
+                <name>{{ config.kerko.meta.title|escape }}</name>
                 <uri>{{ url_for('kerko.search', _external=True)|escape }}</uri>
             </author>
         {%- endblock %}
         <link rel="alternate" type="text/html" href="{{ html_url|escape }}"/>
         <link rel="self" type="application/atom+xml" href="{{ feed_url|escape }}"/>
         {#- RFC 5005 paged feed links #}
         {%- if pager.first %}
@@ -67,12 +67,12 @@
                     {%- if item.data.publisher %}
                         <dc:publisher>{{ item.data.publisher|escape }}</dc:publisher>
                     {%- endif %}
                     {%- if item.data.rights %}
                         <dc:rights>{{ item.data.rights|escape }}</dc:rights>
                     {%- endif %}
                     <dc:title>{{ item.data.title|escape }}</dc:title>
-                {%- endblock %}{# /feed_entry #}
+                {%- endblock feed_entry %}
             </entry>
         {%- endfor %}
-    {%- endblock %}{# /feed_entries #}
+    {%- endblock feed_entries %}
 </feed>
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/base.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/base.html.jinja2`

 * *Files 16% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 <html {%- block html_attributes %}{% if locale %} lang="{{ locale|replace('_', '-') }}"{% endif %} class="no-js"{% endblock %}>
     {%- block head %}
         <head {% block head_attributes %}{% endblock %}>
             {%- block metas %}
                 <meta charset="utf-8"> {# CAUTION: Keep this within the first 1024 characters. #}
                 <meta http-equiv="X-UA-Compatible" content="IE=edge">
             {%- endblock metas %}
-            <title>{% block meta_title_inner %}{{ config.KERKO_TITLE|escape }}{% endblock meta_title_inner %}</title>
+            <title>{% block meta_title_inner %}{{ config.kerko.meta.title|escape }}{% endblock meta_title_inner %}</title>
             {%- block styles %}
             {%- endblock styles %}
             {%- block head_scripts %}
                 {#- Replace the 'no-js' class with 'js' on the root element. -#}
                 <script>
                     var re = new RegExp('(^|\\s)no-js(\\s|$)');
                     document.documentElement.className = document.documentElement.className.replace(re, '$1js$2');
                 </script>
-                {%- if config.GOOGLE_ANALYTICS_ID %}
+                {%- if not config.DEBUG and config.kerko.meta.google_analytics_id %}
                     <!-- Global site tag (gtag.js) - Google Analytics -->
-                    <script async src="https://www.googletagmanager.com/gtag/js?id={{ config.GOOGLE_ANALYTICS_ID }}"></script>
+                    <script async src="https://www.googletagmanager.com/gtag/js?id={{ config.kerko.meta.google_analytics_id }}"></script>
                     <script>
                         window.dataLayer = window.dataLayer || [];
                         function gtag(){dataLayer.push(arguments);}
                         gtag('js', new Date());
-                        gtag('config', '{{ config.GOOGLE_ANALYTICS_ID }}');
+                        gtag('config', '{{ config.kerko.meta.google_analytics_id }}');
                     </script>
                 {%- endif %}
             {%- endblock head_scripts %}
             {%- block favicon %}
             {%- endblock favicon %}
         </head>
     {%- endblock head %}
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 %- block html_attributes %}{% if locale %} lang="{{ locale|replace('_', '-')
 }}"{% endif %} class="no-js"{% endblock %}> {%- block head %}
 % block head_attributes %}{% endblock %}> {%- block metas %}
  {# CAUTION: Keep this within the first 1024 characters. #}
  {%- endblock metas %}
 {%- block styles %} {%- endblock styles %} {%- block head_scripts %} {#-
 Replace the 'no-js' class with 'js' on the root element. -#}
- {%- if config.GOOGLE_ANALYTICS_ID %}
+ {%- if not config.DEBUG and config.kerko.meta.google_analytics_id %}
  {%- endif %} {%- endblock head_scripts %} {%- block favicon %} {%- endblock
 favicon %}
 {%- endblock head %} {%- block body %}
 % block body_attributes %}{% endblock %}> {%- block body_inner %} {%- endblock
 body_inner %} {%- block body_scripts %} {%- endblock body_scripts %}
 {%- endblock body %}
 {%- endblock doc -%}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/item.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/item.html.jinja2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends config.KERKO_TEMPLATE_LAYOUT %}
+{% extends config.kerko.templates.layout %}
 {% from "kerko/_attributes.html.jinja2" import title_aria_label %}
 {% from "kerko/_badges.html.jinja2" import badges %}
 {% from "kerko/_facets.html.jinja2" import facet_items %}
 
 {% macro field(label_text, value_text, field_class=None, value_class=None) %}
     {%- if value_text %}
         <div class="row mb-3 {{ field_class if field_class }}">
@@ -10,16 +10,16 @@
             <div class="col-md-8 col-lg-9 break-word {{ value_class if value_class }}">{{ value_text }}</div>
         </div>
     {%- endif %}
 {%- endmacro %}
 
 {% macro facet_field(label_text, value_text, key, add_title=None) %}
     {#- Display a field using its facet, if available, otherwise fallback to a regular field display. #}
-    {%- if key in config.KERKO_COMPOSER.facets and key in item.facet_results %}
-        {%- set f = config.KERKO_COMPOSER.facets[key] %}
+    {%- if key in config.kerko_composer.facets and key in item.facet_results %}
+        {%- set f = config.kerko_composer.facets[key] %}
         {#- We have a matching facet, display its link. #}
         {{- field(
                 f.title,
                 facet_items(
                     f.missing_label,
                     item.facet_results[f.key],
                     list_tag='div',
@@ -39,74 +39,84 @@
 {% macro permalink(url) -%}
     <a rel="bookmark" title="{{ _('Permanent link to this bibliographic record') }}" href="{{ url }}">{{ url }}</a>
 {%- endmacro -%}
 
 {%- block metas %}
     {{- super() }}
     <link rel="canonical" title="{{ title|escape }}" href="{{ item_url }}">
-    {%- for citation_format in config.KERKO_COMPOSER.get_ordered_specs('citation_formats') %}
+    {%- for citation_format in config.kerko_composer.get_ordered_specs('citation_formats') %}
         <link rel="alternate" title="{{ citation_format.label|escape }}" type="{{ citation_format.mime_type|escape }}" href="{{ url_for('kerko.item_citation_download', item_id=item.id, citation_format_key=citation_format.key) }}">
     {%- endfor %}
     {%- for tag in highwirepress_tags %}
         <meta name="{{ tag[0] }}" content="{{ tag[1]|striptags|escape }}">
     {%- endfor %}
 {%- endblock metas %}
 
 {%- block content_inner %}
     <div class="mt-2 mb-4 item-content">
         {%- block item_actions %}
-            {%- if item.attachments or config.KERKO_PRINT_ITEM_LINK or config.KERKO_COMPOSER.citation_formats %}
+            {%- if item.attachments or config.kerko.features.print_item_link or config.kerko_composer.citation_formats or config.kerko.features.open_in_zotero_app or config.kerko.features.open_in_zotero_web %}
                 <div class="row my-2">
                     <div class="col-auto ml-auto text-right">
                         {%- if item.attachments|length > 1 %}
                             <div class="{% block attachment_links_wrapper_classes %}d-inline-block d-print-none mb-2{% endblock %}">
                                 <div class="dropdown">
                                     <button class="{% block attachment_links_btn_classes %}btn btn-primary dropdown-toggle{% endblock %}" type="button" id="attachment-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                         <span class="fas fa-file" aria-hidden="true"></span> {{ _('Read documents') -}}
                                     </button>
                                     <div class="dropdown-menu dropdown-menu-right dropdown-width-300" aria-labelledby="attachment-options">
                                         {%- for attachment in item.attachments %}
-                                            <a class="dropdown-item" href="{{ url_for('kerko.child_attachment_download', item_id=item.id, attachment_id=attachment['id'], attachment_filename=attachment['data']['filename']) }}"{% if config.KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW %} target="_blank"{% endif %}>
+                                            <a class="dropdown-item" href="{{ url_for('kerko.child_attachment_download', item_id=item.id, attachment_id=attachment['id'], attachment_filename=attachment['data']['filename']) }}"{% if config.kerko.features.download_attachment_new_window %} target="_blank"{% endif %}>
                                                 {{- attachment['data']['filename']|escape }}
                                             </a>
                                         {%- endfor %}
                                     </div>
                                 </div>
                             </div>
                         {%- elif item.attachments|length == 1 %}
                             <div class="{% block attachment_link_wrapper_classes %}d-inline-block d-print-none mb-2{% endblock %}">
-                                <a class="{% block attachment_link_btn_classes %}btn btn-primary{% endblock %}" href="{{ url_for('kerko.child_attachment_download', item_id=item.id, attachment_id=item.attachments[0]['id'], attachment_filename=item.attachments[0]['data']['filename']) }}"{% if config.KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW %} target="_blank"{% endif %} {{ title_aria_label(_('Read \'{}\'').format(item.attachments[0]['data']['filename']|escape)) }}>
+                                <a class="{% block attachment_link_btn_classes %}btn btn-primary{% endblock %}" href="{{ url_for('kerko.child_attachment_download', item_id=item.id, attachment_id=item.attachments[0]['id'], attachment_filename=item.attachments[0]['data']['filename']) }}"{% if config.kerko.features.download_attachment_new_window %} target="_blank"{% endif %} {{ title_aria_label(_('Read \'{}\'').format(item.attachments[0]['data']['filename']|escape)) }}>
                                     <span class="fas fa-file" aria-hidden="true"></span> {{ _('Read document') -}}
                                 </a>
                             </div>
                         {%- endif %}
-                        {%- if config.KERKO_PRINT_ITEM_LINK %}
+                        {%- if config.kerko.features.print_item_link %}
                             <div class="{% block print_link_wrapper_classes %}d-none d-md-inline-block d-print-none mb-2{% endblock %}">
                                 <button id="print-link" class="{% block print_btn_classes %}btn btn-light{% endblock %}" type="button">
                                     <span class="fas fa-print" aria-hidden="true"></span> {{ _('Print this record') }}
                                 </button>
                             </div>
                         {%- endif %}
-                        {%- if config.KERKO_COMPOSER.citation_formats %}
+                        {%- if config.kerko_composer.citation_formats %}
                             <div class="{% block download_link_wrapper_classes %}d-inline-block d-print-none mb-2{% endblock %}">
                                 <div class="dropdown">
-                                    <button class="{% block download_btn_classes %}btn btn-secondary btn-light dropdown-toggle{% endblock %}" type="button" id="download-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                                    <button class="{% block download_btn_classes %}btn btn-light dropdown-toggle{% endblock %}" type="button" id="download-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                         <span class="fas fa-download" aria-hidden="true"></span> {% trans count=1, count_formatted='1' %}Download this record{% pluralize %}Download {{ count_formatted }} records{% endtrans -%} {# TODO: Remove pluralization after solving issue where translation is not loaded when the same message is sometimes pluralized, sometimes not. -#}
                                     </button>
                                     <div class="dropdown-menu dropdown-menu-right dropdown-width-300" aria-labelledby="download-options">
-                                        {%- for citation_format in config.KERKO_COMPOSER.get_ordered_specs('citation_formats') %}
+                                        {%- for citation_format in config.kerko_composer.get_ordered_specs('citation_formats') %}
                                             <a class="dropdown-item" href="{{ url_for('kerko.item_citation_download', item_id=item.id, citation_format_key=citation_format.key) }}" rel="alternate" type="{{ citation_format.mime_type|escape }}" {{ title_aria_label(_('Download in {download_option} format').format(download_option=citation_format.label|escape)) }}>
                                                 {{- citation_format.label -}}
                                             </a>
                                             <p class="px-4 text-muted">{{ citation_format.help_text }}</p>
                                         {%- endfor %}
                                     </div>
                                 </div>
                             </div>
                         {%- endif %}
+                        {%- if config.kerko.features.open_in_zotero_app and open_in_zotero_app_url %}
+                            <div id="open-in-zotero-app" class="text-right d-inline-block d-print-none mb-2 {% if not open_in_zotero_app %}d-none-important{% endif %}">
+                                <a class="btn btn-light" href="{{ open_in_zotero_app_url }}"><span class="fas fa-external-link-alt" aria-hidden="true"></span> {{ _("Open in Zotero") }}</a>
+                            </div>
+                        {%- endif %}
+                        {%- if config.kerko.features.open_in_zotero_web and open_in_zotero_web_url %}
+                            <div id="open-in-zotero-web" class="text-right d-inline-block d-print-none mb-2 {% if not open_in_zotero_web %}d-none-important{% endif %}">
+                                <a class="btn btn-light" href="{{ open_in_zotero_web_url }}" target="_blank"><span class="fas fa-external-link-alt" aria-hidden="true"></span> {{ _("View on zotero.org") }}</a>
+                            </div>
+                        {%- endif %}
                     </div>
                 </div>
             {%- endif %}
         {%- endblock item_actions %}
         {%- block item_field_resource_type %}
             {{- facet_field(_("Resource type"), item.item_type_label, 'facet_item_type', add_title=_("Search the '{}' resource type").format(item.item_type_label)) }}
         {%- endblock item_field_resource_type %}
@@ -167,68 +177,68 @@
             {{- field(_("Notes"), item.notes|join('')|safe) if item.notes }}
         {%- endblock item_field_notes %}
         {%- block item_field_citation %}
             {{- field(_("Citation"), ('<div class="card"><div class="card-body">' + item.bib + '</div></div>')|safe) }}
         {%- endblock item_field_citation %}
         {%- block item_facets %}
             {%- if item.facet_results %}
-                {%- for f in config.KERKO_COMPOSER.get_ordered_specs('facets') if f.item_view and f.key in item.facet_results %}
+                {%- for f in config.kerko_composer.get_ordered_specs('facets') if f.item_view and f.key in item.facet_results %}
                     {{ f.render(item.facet_results[f.key], 'field') }}
                 {%- endfor %}
             {%- endif %}
         {%- endblock item_facets %}
         {%- block item_field_attachments %}
             {%- if item.attachments %}
                 <div class="row">
                     <div class="col-md-4 col-lg-3 font-weight-bold break-word text-md-right text-print-left">{% trans count=item.attachments|length %}Document{% pluralize %}Documents{% endtrans %}</div>
                     <div class="col-md-8 col-lg-9 break-word">
                         <ul class="list-unstyled">
                             {%- for attachment in item.attachments %}
-                                <li><a href="{{ url_for('kerko.child_attachment_download', item_id=item.id, attachment_id=attachment['id'], attachment_filename=attachment['data']['filename']) }}"{% if config.KERKO_DOWNLOAD_ATTACHMENT_NEW_WINDOW %} target="_blank"{% endif %}><span class="fas fa-file d-print-none no-decorate mr-1" aria-hidden="true"></span>{{ attachment['data']['filename']|escape }}</a></li>
+                                <li><a href="{{ url_for('kerko.child_attachment_download', item_id=item.id, attachment_id=attachment['id'], attachment_filename=attachment['data']['filename']) }}"{% if config.kerko.features.download_attachment_new_window %} target="_blank"{% endif %}><span class="fas fa-file d-print-none no-decorate mr-1" aria-hidden="true"></span>{{ attachment['data']['filename']|escape }}</a></li>
                             {%- endfor %}
                         </ul>
                     </div>
                 </div>
             {%- endif %}
         {%- endblock item_field_attachments %}
         {%- block item_field_permalink %}
             {{- field(_("Link to this record"), permalink(item_url)) }}
         {%- endblock item_field_permalink %}
         {%- block item_field_relations %}
             {#- Determine which relation tab is to be initially active, if any. #}
             {%- set relations_ns = namespace(active_tab=None) %}
-            {%- for rel in config.KERKO_COMPOSER.get_ordered_specs('relations') %}
+            {%- for rel in config.kerko_composer.get_ordered_specs('relations') %}
                 {%- if not relations_ns.active_tab %}
                     {%- if item[rel.field.key] %}
                         {%- set relations_ns.active_tab = rel.key %}
                     {%- elif rel.reverse and item[rel.reverse_field_key] %}
                         {%- set relations_ns.active_tab = rel.reverse_key %}
                     {%- endif %}
                 {%- endif %}
             {%- endfor %}
             {%- if relations_ns.active_tab %}
                 <div class="row">
                     <div class="col-md-4 col-lg-3 font-weight-bold break-word text-md-right mb-2 mt-md-2 d-print-none">{{ _('Relations') }}</div>
                     <div class="col-md-8 col-lg-9 break-word">
                         <ul class="nav nav-tabs d-print-none" role="tablist">
-                            {%- for rel in config.KERKO_COMPOSER.get_ordered_specs('relations') %}
+                            {%- for rel in config.kerko_composer.get_ordered_specs('relations') %}
                                 {%- if item[rel.field.key] %}
                                     <li class="nav-item" role="tab">
                                         <a id="tab-{{ rel.key }}" href="#{{ rel.key }}" class="nav-link {% if rel.key == relations_ns.active_tab %}active{% endif %}" data-toggle="tab" aria-controls="{{ rel.key }}" {% if rel.key == relations_ns.active_tab %}aria-selected="true"{% endif %}>{{ rel.label }}</a>
                                     </li>
                                 {%- endif %}
                                 {%- if rel.reverse and item[rel.reverse_field_key] %}
                                     <li class="nav-item" role="tab">
                                         <a id="tab-{{ rel.reverse_key }}" href="#{{ rel.reverse_key }}" class="nav-link {% if rel.reverse_key == relations_ns.active_tab %}active{% endif %}" data-toggle="tab" aria-controls="{{ rel.reverse_key }}" {% if rel.reverse_key == relations_ns.active_tab %}aria-selected="true"{% endif %}>{{ rel.reverse_label }}</a>
                                     </li>
                                 {%- endif %}
                             {%- endfor %}
                         </ul>
                         <div class="tab-content">
-                            {%- for rel in config.KERKO_COMPOSER.get_ordered_specs('relations') %}
+                            {%- for rel in config.kerko_composer.get_ordered_specs('relations') %}
                                 {%- if item[rel.field.key] %}
                                     {%- with key=rel.key, field=rel.field.key, label=rel.label, is_active=rel.key == relations_ns.active_tab %}
                                         {%- include "kerko/_item-relations.html.jinja2" %}
                                     {%- endwith %}
                                 {%- endif %}
                                 {%- if rel.reverse and item[rel.reverse_field_key] %}
                                     {%- with key=rel.reverse_key, field=rel.reverse_field_key, label=rel.reverse_label, is_active=rel.reverse_key == relations_ns.active_tab %}
@@ -249,14 +259,30 @@
 
 {%- block content_footer %}
     {%- if config.DEBUG %}
         <div class="text-right mb-4 mt-2 text-muted">{% trans time="%.2f"|format(time) %}Processing time: {{time}} seconds{% endtrans %}</div>
     {%- endif %}
 {%- endblock content_footer %}
 
+{%- block footer_inner %}
+    {{ super() }}
+    {%- block preferences %}
+        {%- if config.kerko.features.open_in_zotero_app or config.kerko.features.open_in_zotero_web %}
+            <div class="text-right d-print-none pr-3 pb-3">
+                <button class="btn btn-secondary" data-toggle="modal" data-target="#preferences-modal">
+                    <span class="fas fa-cog" aria-hidden="true"></span> {{ _("Preferences") }}
+                </button>
+            </div>
+            <div class="text-dark d-print-none">
+                {%- include "kerko/_preferences.html.jinja2" %}
+            </div>
+        {%- endif %}
+    {%- endblock preferences %}
+{%- endblock footer_inner %}
+
 {%- block content_header %}
     <div class="row">
         <div class="{% block top_link_wrapper_classes %}col-auto ml-auto my-2 d-print-none{% endblock %}">
             <a class="{% block top_btn_classes %}btn btn-primary{% endblock %}" href="{{ url_for('kerko.search') }}">
                 <span class="fas fa-arrow-up" aria-hidden="true"></span> {{ _("Full bibliography") }}
             </a>
         </div>
@@ -271,14 +297,17 @@
     </div>
 {%- endblock content_header %}
 
 {%- block body_scripts %}
     {{- super() }}
     {%- block kerko_item_js %}
         <script src="{{ url_for('kerko.static', filename='kerko/js/item.js') }}?202008101934"></script>
+        {%- if config.kerko.features.open_in_zotero_app or config.kerko.features.open_in_zotero_web %}
+            <script src="{{ url_for('kerko.static', filename='kerko/js/open_in_zotero.js') }}?20221016"></script>
+        {%- endif %}
     {%- endblock kerko_item_js %}
     {%- block kerko_print_js %}
-        {%- if config.KERKO_PRINT_ITEM_LINK %}
+        {%- if config.kerko.features.print_item_link %}
             <script src="{{ url_for('kerko.static', filename='kerko/js/print.js') }}"></script>
         {%- endif %}
     {%- endblock kerko_print_js %}
 {%- endblock body_scripts %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/layout.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/layout.html.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends config.KERKO_TEMPLATE_BASE %}
+{% extends config.kerko.templates.base %}
 {% from "kerko/_attributes.html.jinja2" import title_aria_label %}
 
 {%- block meta_title_inner -%}
     {%- if title %}{{ title|escape }} | {% endif %}{{ super() -}}
 {%- endblock %}
 
 {%- block metas %}
@@ -11,24 +11,24 @@
     <meta name="generator" content="Kerko">
 {%- endblock metas %}
 
 {%- block styles %}
     {{- super() }}
     {%- block bootstrap_css %}
         {%- if bootstrap %}
-            {{ bootstrap.load_css(version=config.KERKO_BOOTSTRAP_VERSION) }}
+            {{ bootstrap.load_css(version=config.kerko.assets.bootstrap_version) }}
         {%- endif %}
     {%- endblock bootstrap_css %}
     {%- block fontawesome_css %}
         <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/solid.css" integrity="sha384-ioUrHig76ITq4aEJ67dHzTvqjsAP/7IzgwE7lgJcg2r7BRNGYSK0LwSmROzYtgzs" crossorigin="anonymous">
         <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/regular.css" integrity="sha384-hCIN6p9+1T+YkCd3wWjB5yufpReULIPQ21XA/ncf3oZ631q2HEhdC7JgKqbk//4+" crossorigin="anonymous">
         <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/fontawesome.css" integrity="sha384-sri+NftO+0hcisDKgr287Y/1LVnInHJ1l+XC7+FOabmTTIK0HnE2ID+xxvJ21c5J" crossorigin="anonymous">
     {%- endblock fontawesome_css %}
     {%- block kerko_css %}
-        <link rel="stylesheet" href="{{ url_for('kerko.static', filename='kerko/css/styles.css') }}?20221229">
+        <link rel="stylesheet" href="{{ url_for('kerko.static', filename='kerko/css/styles.css') }}?20230626">
     {%- endblock kerko_css %}
 {%- endblock styles %}
 
 {%- block body_inner %}
     {%- block header %}
         <header {% block header_attributes %}{% endblock %}>
             {%- block header_inner %}
@@ -109,15 +109,15 @@
 {%- endblock body_inner %}
 
 {%- block body_scripts %}
     {{- super() }}
     {%- block bootstrap_js %}
         {%- if bootstrap %}
             {{ bootstrap.load_js(
-                version=config.KERKO_BOOTSTRAP_VERSION,
-                jquery_version=config.KERKO_JQUERY_VERSION,
-                popper_version=config.KERKO_POPPER_VERSION,
-                with_jquery=config.KERKO_WITH_JQUERY,
-                with_popper=config.KERKO_WITH_POPPER) }}
+                version=config.kerko.assets.bootstrap_version,
+                jquery_version=config.kerko.assets.jquery_version,
+                popper_version=config.kerko.assets.popper_version,
+                with_jquery=config.kerko.assets.with_jquery,
+                with_popper=config.kerko.assets.with_popper) }}
         {%- endif %}
     {%- endblock bootstrap_js %}
 {%- endblock body_scripts %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/search-item.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/search-item.html.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% set apply_relations_initial_limit = True %}
-{% extends config.KERKO_TEMPLATE_ITEM %}
+{% extends config.kerko.templates.item %}
 
 {%- block metas %}
     {{- super() }}
     {%- include "kerko/_search-metas.html.jinja2" %}
 {%- endblock metas %}
 
 {%- block content_header %}
```

### Comparing `Kerko-0.9/src/kerko/templates/kerko/search.html.jinja2` & `Kerko-1.0.0a0/src/kerko/templates/kerko/search.html.jinja2`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-{% extends config.KERKO_TEMPLATE_LAYOUT %}
+{% extends config.kerko.templates.layout %}
 {% from "kerko/_attributes.html.jinja2" import title_aria_label %}
 
-{%- set show_print_link = config.KERKO_PRINT_CITATIONS_MAX_COUNT == 0 or total_count <= config.KERKO_PRINT_CITATIONS_MAX_COUNT %}
-{%- set show_print_link = show_print_link and config.KERKO_PRINT_CITATIONS_LINK %}
-{%- set show_download_link = config.KERKO_DOWNLOAD_CITATIONS_MAX_COUNT == 0 or total_count <= config.KERKO_DOWNLOAD_CITATIONS_MAX_COUNT %}
-{%- set show_download_link = show_download_link and config.KERKO_DOWNLOAD_CITATIONS_LINK and config.KERKO_COMPOSER.citation_formats %}
+{%- set show_print_link = config.kerko.features.print_citations_max_count == 0 or total_count <= config.kerko.features.print_citations_max_count %}
+{%- set show_print_link = show_print_link and config.kerko.features.print_citations_link %}
+{%- set show_download_link = config.kerko.features.download_citations_max_count == 0 or total_count <= config.kerko.features.download_citations_max_count %}
+{%- set show_download_link = show_download_link and config.kerko.features.download_citations_link and config.kerko_composer.citation_formats %}
 {%- set abstracts_toggler_title = _('Hide abstracts') if show_abstracts else _('Show abstracts') %}
 
 {%- block metas %}
     {{- super() }}
     {%- include "kerko/_search-metas.html.jinja2" %}
 {%- endblock metas %}
 
@@ -74,24 +74,24 @@
                     <div class="d-inline-block d-print-none">
                         {%- include "kerko/_sorter.html.jinja2" %}
                     </div>
                 </div>
             {%- endif %}
         </div>
         {%- if search_results %}
-            {%- if pager or config.KERKO_RESULTS_ABSTRACTS_TOGGLER %}
+            {%- if pager or config.kerko.features.results_abstracts_toggler %}
                 <div class="row mb-2">
                     {%- if pager %}
                         <div class="col-auto mr-auto">
                             {%- block pager_top %}
                                 {%- include "kerko/_pager.html.jinja2" %}
                             {%- endblock pager_top %}
                         </div>
                     {%- endif %}
-                    {%- if config.KERKO_RESULTS_ABSTRACTS_TOGGLER %}
+                    {%- if config.kerko.features.results_abstracts_toggler %}
                         <div class="col-auto ml-auto pl-0">
                             {%- block abstracts_toggler %}
                                 <a class="btn btn-light d-print-none" href="{{ abstracts_toggler_url }}" title="{{ abstracts_toggler_title }}" aria-label="{{ abstracts_toggler_title }}">{% if show_abstracts %}<span class="fas fa-toggle-on" aria-hidden="true"></span>{% else %}<span class="fas fa-toggle-off" aria-hidden="true"></span>{% endif %} {{ _("Abstracts") }}</a>
                             {%- endblock abstracts_toggler %}
                         </div>
                     {%- endif %}
                 </div>
@@ -120,15 +120,15 @@
                             {%- if show_download_link %}
                                 <div class="{% block download_link_wrapper_classes %}d-inline-block d-print-none mb-1{% endblock %}">
                                     <div class="dropdown">
                                         <button class="{% block download_btn_classes %}btn btn-secondary btn-light dropdown-toggle{% endblock %}" type="button" id="download-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                             <span class="fas fa-download" aria-hidden="true"></span> {% trans count=total_count, count_formatted=total_count_formatted|safe %}Download this record{% pluralize %}Download {{ count_formatted }} records{% endtrans -%}
                                         </button>
                                         <div class="dropdown-menu dropdown-menu-right dropdown-width-300" aria-labelledby="download-options">
-                                            {%- for citation_format in config.KERKO_COMPOSER.get_ordered_specs('citation_formats') %}
+                                            {%- for citation_format in config.kerko_composer.get_ordered_specs('citation_formats') %}
                                                 <a class="dropdown-item" href="{{ download_urls[citation_format.key] }}" rel="nofollow" type="{{ citation_format.mime_type|escape }}" {{ title_aria_label(_('Download in {download_option} format').format(download_option=citation_format.label|escape)) }}>
                                                     {{- citation_format.label -}}
                                                 </a>
                                                 <p class="px-4 text-muted">{{ citation_format.help_text }}</p>
                                             {%- endfor %}
                                         </div>
                                     </div>
@@ -168,15 +168,15 @@
 
 {%- block sidebar_inner %}
     {%- block facet_results %}
         {%- if facet_results and search_results %}
             <div id="facets-container" class="d-none d-lg-block d-print-none">
                 <h2 class="{% block facets_heading_classes %}mt-2 mb-4{% endblock %}">{{ _("Explore") }}</h2>
                 <div id="facets" class="facets">
-                    {%- for f in config.KERKO_COMPOSER.get_ordered_specs('facets') %}
+                    {%- for f in config.kerko_composer.get_ordered_specs('facets') %}
                         {{ f.render(facet_results[f.key], 'search') }}
                     {%- endfor %}
                 </div>
             </div>
             <div id="facets-modal" class="modal fade" tabindex="-1" role="dialog" aria-labelledby="facets-modal-label" aria-hidden="true">
                 <div class="modal-dialog modal-lg modal-dialog-scrollable" role="document">
                     <div class="modal-content">
```

### Comparing `Kerko-0.9/src/kerko/text.py` & `Kerko-1.0.0a0/src/kerko/text.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/transformers.py` & `Kerko-1.0.0a0/src/kerko/transformers.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/translations/de/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Sven Rothe <mmoole@gmail.com>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid ""
 "\n"
 "                <p>Suggestions:</p>\n"
 "                <ul>\n"
 "                    <li>Make sure that all words are spelled correctly.</"
 "li>\n"
```

### Comparing `Kerko-0.9/src/kerko/translations/de/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.po`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/translations/fr/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kerko\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-12-10 20:25-0500\n"
-"PO-Revision-Date: 2022-12-10 20:25-0500\n"
+"POT-Creation-Date: 2023-05-12 16:19-0400\n"
+"PO-Revision-Date: 2023-05-12 16:19-0400\n"
 "Last-Translator: David Lesieur <kerko@whiskyechobravo.com>\n"
 "Language: fr\n"
 "Language-Team: fr <kerko@whiskyechobravo.com>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid ""
 "\n"
 "                <p>Suggestions:</p>\n"
 "                <ul>\n"
 "                    <li>Make sure that all words are spelled correctly.</"
 "li>\n"
@@ -28,14 +28,17 @@
 "                <ul>\n"
 "                    <li>Vérifiez que tous les mots sont orthographiés "
 "correctement.</li>\n"
 "                    <li>Essayez des termes différents.</li>\n"
 "                    <li>Essayez des termes plus généraux.</li>\n"
 "                </ul>"
 
+msgid "\"{}\" button"
+msgstr "Bouton « {} »"
+
 msgid "%(count_formatted)s resource"
 msgid_plural "%(count_formatted)s resources"
 msgstr[0] "%(count_formatted)s ressource"
 msgstr[1] "%(count_formatted)s ressources"
 
 msgid ": "
 msgstr "&nbsp;: "
@@ -153,14 +156,17 @@
 
 msgid "Close Explore panel"
 msgstr "Fermer le panneau d’exploration"
 
 msgid "Close Help panel"
 msgstr "Fermer le panneau d’aide"
 
+msgid "Close preferences"
+msgstr "Fermer les préférences"
+
 msgid "Collapse subfilters"
 msgstr "Masquer les filtres plus spécifiques"
 
 msgid "Current page"
 msgstr "Page courante"
 
 msgid "Current sort"
@@ -280,26 +286,32 @@
 
 msgid "Oldest first"
 msgstr "Date croissante"
 
 msgid "Online resource"
 msgstr "Ressource en ligne"
 
+msgid "Open in Zotero"
+msgstr "Ouvrir dans Zotero"
+
 msgid "Page %(current)s of %(total)s"
 msgstr "Page %(current)s de %(total)s"
 
 msgid "Page %(page_num)s"
 msgstr "Page %(page_num)s"
 
 msgid "Permanent link to this bibliographic record"
 msgstr "Lien permanent vers cette notice bibliographique"
 
 msgid "Powered by {zotero} and {kerko}."
 msgstr "Propulsé par {zotero} et {kerko}."
 
+msgid "Preferences"
+msgstr "Préférences"
+
 msgid "Previous page"
 msgstr "Page précédente"
 
 msgid "Print this citation"
 msgid_plural "Print %(count_formatted)s citations"
 msgstr[0] "Imprimer cette référence"
 msgstr[1] "Imprimer %(count_formatted)s références"
@@ -418,14 +430,36 @@
 
 msgid "Show less"
 msgstr "Montrer moins"
 
 msgid "Show more"
 msgstr "Montrer plus"
 
+msgid ""
+"Show or hide the \"{}\" button on full bibliographic record pages. This "
+"button allows you to open the record in the Zotero application. It might be "
+"useful only if you have the Zotero application installed on your device, and "
+"if you were granted access to the Zotero library that holds the record."
+msgstr ""
+"Montrer ou cacher le bouton « {} » sur les pages de notices "
+"bibliographiques. Ce bouton vous permet d’ouvrir la notice dans le logiciel "
+"Zotero. Celui-ci ne peut être utile que si vous avez installé le logiciel "
+"Zotero sur votre appareil et si vous avez obtenu la permission d’accéder à "
+"la bibliothèque Zotero dans laquelle est consignée la notice."
+
+msgid ""
+"Show or hide the \"{}\" button on full bibliographic record pages. This "
+"button allows you to view the record on zotero.org. It might be useful only "
+"if you were granted access to the Zotero library that holds the record."
+msgstr ""
+"Montrer ou cacher le bouton « {} » sur les pages de notices "
+"bibliographiques. Ce bouton vous permet de consulter la notice sur zotero."
+"org. Celui-ci ne peut être utile que si vous avez obtenu la permission "
+"d’accéder à la bibliothèque Zotero dans laquelle est consignée la notice."
+
 msgid "Sort by {sort_option}"
 msgstr "Trier par {sort_option}"
 
 msgid "Sort by..."
 msgstr "Trier par..."
 
 msgid "Sort by: {sort_option}"
@@ -580,14 +614,17 @@
 "apparaît par exemple dans le titre d’une référence, le score de cette "
 "référence sera plus élevé que s’il apparaissait dans un champ moins "
 "important tel le résumé."
 
 msgid "View details"
 msgstr "Voir les détails"
 
+msgid "View on zotero.org"
+msgstr "Voir sur zotero.org"
+
 msgid "View on {}"
 msgstr "Consulter sur {}"
 
 msgid ""
 "You may control the extent of your search by selecting where to search. The "
 "options are:"
 msgstr ""
```

### Comparing `Kerko-0.9/src/kerko/translations/fr/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # French translations for Kerko.
-# Copyright (C) 2022 Kerko Contributors
+# Copyright (C) 2023 Kerko Contributors
 # This file is distributed under the same license as the Kerko project.
-# David Lesieur <kerko@whiskyechobravo.com>, 2022.
+# David Lesieur <kerko@whiskyechobravo.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kerko\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-12-10 20:25-0500\n"
-"PO-Revision-Date: 2022-12-10 20:25-0500\n"
+"POT-Creation-Date: 2023-05-12 16:19-0400\n"
+"PO-Revision-Date: 2023-05-12 16:19-0400\n"
 "Last-Translator: David Lesieur <kerko@whiskyechobravo.com>\n"
 "Language: fr\n"
 "Language-Team: fr <kerko@whiskyechobravo.com>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: src/kerko/codecs.py:92
 msgid "yes"
 msgstr "oui"
 
 #: src/kerko/codecs.py:92
 msgid "no"
@@ -74,105 +74,105 @@
 msgid "In documents"
 msgstr "Dans les documents"
 
 #: src/kerko/composer.py:293
 msgid "Search your keywords in the text content of the available documents."
 msgstr "repère vos mots-clés dans le contenu textuel des documents disponibles."
 
-#: src/kerko/composer.py:1549
+#: src/kerko/composer.py:1587
 msgid "Topic"
 msgstr "Sujet"
 
-#: src/kerko/composer.py:1572 src/kerko/templates/kerko/item.html.jinja2:111
+#: src/kerko/composer.py:1610 src/kerko/templates/kerko/item.html.jinja2:121
 msgid "Resource type"
 msgstr "Type de ressource"
 
-#: src/kerko/composer.py:1592
+#: src/kerko/composer.py:1630
 msgid "Publication year"
 msgstr "Année de publication"
 
-#: src/kerko/composer.py:1600
+#: src/kerko/composer.py:1638
 msgid "Unknown"
 msgstr "Inconnue"
 
-#: src/kerko/composer.py:1612
+#: src/kerko/composer.py:1650
 msgid "Online resource"
 msgstr "Ressource en ligne"
 
-#: src/kerko/composer.py:1643
+#: src/kerko/composer.py:1681
 msgid "Relevance"
 msgstr "Pertinence"
 
-#: src/kerko/composer.py:1654
+#: src/kerko/composer.py:1692
 msgid "Newest first"
 msgstr "Date décroissante"
 
-#: src/kerko/composer.py:1672
+#: src/kerko/composer.py:1710
 msgid "Oldest first"
 msgstr "Date croissante"
 
-#: src/kerko/composer.py:1685
+#: src/kerko/composer.py:1723
 msgid "Author A-Z"
 msgstr "Auteur A-Z"
 
-#: src/kerko/composer.py:1698
+#: src/kerko/composer.py:1736
 msgid "Author Z-A"
 msgstr "Auteur Z-A"
 
-#: src/kerko/composer.py:1716
+#: src/kerko/composer.py:1754
 msgid "Title A-Z"
 msgstr "Titre A-Z"
 
-#: src/kerko/composer.py:1729
+#: src/kerko/composer.py:1767
 msgid "Title Z-A"
 msgstr "Titre Z-A"
 
-#: src/kerko/composer.py:1761
+#: src/kerko/composer.py:1799
 msgid "RIS"
 msgstr "RIS"
 
-#: src/kerko/composer.py:1762
+#: src/kerko/composer.py:1800
 msgid "Recommended format for most reference management software"
 msgstr ""
 "Format recommandé pour la plupart des logiciels de gestion de références "
 "bibliographiques"
 
-#: src/kerko/composer.py:1773
+#: src/kerko/composer.py:1811
 msgid "BibTeX"
 msgstr "BibTeX"
 
-#: src/kerko/composer.py:1774
+#: src/kerko/composer.py:1812
 msgid "Recommended format for BibTeX-specific software"
 msgstr "Format recommandé pour les logiciels spécialement conçus pour BibTeX"
 
-#: src/kerko/composer.py:1798
+#: src/kerko/composer.py:1836
 msgid "Cites"
 msgstr "Cite"
 
-#: src/kerko/composer.py:1804
+#: src/kerko/composer.py:1842
 msgid "Cited by"
 msgstr "Cité par"
 
-#: src/kerko/composer.py:1812
+#: src/kerko/composer.py:1850
 msgid "Related"
 msgstr "Connexe"
 
-#: src/kerko/search.py:107
+#: src/kerko/searcher.py:109
 #: src/kerko/templates/kerko/_search-help.html.jinja2:37
 #: src/kerko/templates/kerko/_search-help.html.jinja2:43
 msgid "AND"
 msgstr "ET"
 
-#: src/kerko/search.py:108
+#: src/kerko/searcher.py:110
 #: src/kerko/templates/kerko/_search-help.html.jinja2:38
 #: src/kerko/templates/kerko/_search-help.html.jinja2:43
 msgid "OR"
 msgstr "OU"
 
-#: src/kerko/search.py:109
+#: src/kerko/searcher.py:111
 #: src/kerko/templates/kerko/_search-help.html.jinja2:39
 msgid "NOT"
 msgstr "SAUF"
 
 #: src/kerko/templates/kerko/_breadbox.html.jinja2:15
 msgid "Remove the '{}' search term"
 msgstr "Retirer le terme '{}'"
@@ -245,14 +245,74 @@
 msgstr "Pagination des résultats de recherche"
 
 #: src/kerko/templates/kerko/_pager.html.jinja2:89
 #, python-format
 msgid "Page %(current)s of %(total)s"
 msgstr "Page %(current)s de %(total)s"
 
+#: src/kerko/templates/kerko/_preferences.html.jinja2:8
+#: src/kerko/templates/kerko/item.html.jinja2:272
+msgid "Preferences"
+msgstr "Préférences"
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:9
+#: src/kerko/templates/kerko/_preferences.html.jinja2:41
+msgid "Close preferences"
+msgstr "Fermer les préférences"
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:22
+#: src/kerko/templates/kerko/_preferences.html.jinja2:32
+msgid "\"{}\" button"
+msgstr "Bouton « {} »"
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:22
+#: src/kerko/templates/kerko/_preferences.html.jinja2:24
+#: src/kerko/templates/kerko/item.html.jinja2:108
+msgid "Open in Zotero"
+msgstr "Ouvrir dans Zotero"
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:24
+msgid ""
+"Show or hide the \"{}\" button on full bibliographic record pages. This "
+"button allows you to open the record in the Zotero application. It might "
+"be useful only if you have the Zotero application installed on your "
+"device, and if you were granted access to the Zotero library that holds "
+"the record."
+msgstr ""
+"Montrer ou cacher le bouton « {} » sur les pages de notices "
+"bibliographiques. Ce bouton vous permet d’ouvrir la notice dans le "
+"logiciel Zotero. Celui-ci ne peut être utile que si vous avez installé le"
+" logiciel Zotero sur votre appareil et si vous avez obtenu la permission "
+"d’accéder à la bibliothèque Zotero dans laquelle est consignée la notice."
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:32
+#: src/kerko/templates/kerko/_preferences.html.jinja2:34
+#: src/kerko/templates/kerko/item.html.jinja2:113
+msgid "View on zotero.org"
+msgstr "Voir sur zotero.org"
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:34
+msgid ""
+"Show or hide the \"{}\" button on full bibliographic record pages. This "
+"button allows you to view the record on zotero.org. It might be useful "
+"only if you were granted access to the Zotero library that holds the "
+"record."
+msgstr ""
+"Montrer ou cacher le bouton « {} » sur les pages de notices "
+"bibliographiques. Ce bouton vous permet de consulter la notice sur "
+"zotero.org. Celui-ci ne peut être utile que si vous avez obtenu la "
+"permission d’accéder à la bibliothèque Zotero dans laquelle est "
+"consignée la notice."
+
+#: src/kerko/templates/kerko/_preferences.html.jinja2:41
+#: src/kerko/templates/kerko/_search-help.html.jinja2:72
+#: src/kerko/templates/kerko/search.html.jinja2:191
+msgid "Close"
+msgstr "Fermer"
+
 #: src/kerko/templates/kerko/_search-form.html.jinja2:8
 msgid "Search within results for..."
 msgstr "Chercher parmi les résultats..."
 
 #: src/kerko/templates/kerko/_search-form.html.jinja2:8
 msgid "Search for..."
 msgstr "Chercher les mots-clés..."
@@ -620,19 +680,14 @@
 "effect on the relevance score. Their only effect is to filter the list of"
 " results."
 msgstr ""
 "Les catégories sélectionnées dans la section <strong>{explore}</strong> "
 "n’ont aucun effet sur le tri par pertinence. Elles ne font que filtrer la"
 " liste des résultats."
 
-#: src/kerko/templates/kerko/_search-help.html.jinja2:72
-#: src/kerko/templates/kerko/search.html.jinja2:191
-msgid "Close"
-msgstr "Fermer"
-
 #: src/kerko/templates/kerko/_search-result.html.jinja2:14
 msgid "View details"
 msgstr "Voir les détails"
 
 #: src/kerko/templates/kerko/_search-result.html.jinja2:46
 #: src/kerko/templates/kerko/item.html.jinja2:64
 msgid "Read documents"
@@ -685,62 +740,67 @@
 msgstr[1] "Télécharger %(count_formatted)s notices"
 
 #: src/kerko/templates/kerko/item.html.jinja2:97
 #: src/kerko/templates/kerko/search.html.jinja2:128
 msgid "Download in {download_option} format"
 msgstr "Télécharger au format {download_option}"
 
-#: src/kerko/templates/kerko/item.html.jinja2:111
+#: src/kerko/templates/kerko/item.html.jinja2:121
 msgid "Search the '{}' resource type"
 msgstr "Chercher le type de ressource '{}'"
 
-#: src/kerko/templates/kerko/item.html.jinja2:116
+#: src/kerko/templates/kerko/item.html.jinja2:126
 msgid "Author/contributor"
 msgid_plural "Authors/contributors"
 msgstr[0] "Auteur/contributeur"
 msgstr[1] "Auteurs/contributeurs"
 
-#: src/kerko/templates/kerko/item.html.jinja2:121
+#: src/kerko/templates/kerko/item.html.jinja2:131
 msgid "Search '{}'"
 msgstr "Chercher '{}'"
 
-#: src/kerko/templates/kerko/item.html.jinja2:155
+#: src/kerko/templates/kerko/item.html.jinja2:165
 msgid "Link"
 msgid_plural "Links"
 msgstr[0] "Lien"
 msgstr[1] "Liens"
 
-#: src/kerko/templates/kerko/item.html.jinja2:167
+#: src/kerko/templates/kerko/item.html.jinja2:177
 msgid "Notes"
 msgstr "Notes"
 
-#: src/kerko/templates/kerko/item.html.jinja2:170
+#: src/kerko/templates/kerko/item.html.jinja2:180
 msgid "Citation"
 msgstr "Référence"
 
-#: src/kerko/templates/kerko/item.html.jinja2:182
+#: src/kerko/templates/kerko/item.html.jinja2:192
 msgid "Document"
 msgid_plural "Documents"
 msgstr[0] "Document"
 msgstr[1] "Documents"
 
-#: src/kerko/templates/kerko/item.html.jinja2:194
+#: src/kerko/templates/kerko/item.html.jinja2:204
 msgid "Link to this record"
 msgstr "Lien vers cette notice"
 
-#: src/kerko/templates/kerko/item.html.jinja2:210
+#: src/kerko/templates/kerko/item.html.jinja2:220
 msgid "Relations"
 msgstr "Relations"
 
-#: src/kerko/templates/kerko/item.html.jinja2:252
+#: src/kerko/templates/kerko/item.html.jinja2:262
 #: src/kerko/templates/kerko/search.html.jinja2:149
 #, python-format
 msgid "Processing time: %(time)s seconds"
 msgstr "Temps de traitement: %(time)s seconds"
 
+#: src/kerko/templates/kerko/item.html.jinja2:286 src/kerko/views/search.py:122
+#: src/kerko/views/search.py:200
+msgid "Full bibliography"
+msgstr "Bibliographie complète"
+
 #: src/kerko/templates/kerko/layout.html.jinja2:42
 msgid "Toggle navigation"
 msgstr "Basculer la navigation"
 
 #: src/kerko/templates/kerko/layout.html.jinja2:74
 msgid "Remove this message"
 msgstr "Retirer ce message"
@@ -758,15 +818,15 @@
 msgstr "Cacher les résumés"
 
 #: src/kerko/templates/kerko/search.html.jinja2:8
 msgid "Show abstracts"
 msgstr "Montrer les résumés"
 
 #: src/kerko/templates/kerko/search.html.jinja2:19
-#: src/kerko/views/searching.py:113
+#: src/kerko/views/search.py:120
 msgid "Your search"
 msgstr "Votre recherche"
 
 #: src/kerko/templates/kerko/search.html.jinja2:68
 #, python-format
 msgid "%(count_formatted)s resource"
 msgid_plural "%(count_formatted)s resources"
@@ -810,40 +870,36 @@
 "                </ul>"
 
 #: src/kerko/templates/kerko/search.html.jinja2:185
 #: src/kerko/templates/kerko/search.html.jinja2:191
 msgid "Close Explore panel"
 msgstr "Fermer le panneau d’exploration"
 
-#: src/kerko/views/routes.py:118 src/kerko/views/searching.py:241
+#: src/kerko/views/routes.py:131 src/kerko/views/search.py:250
 msgid "Custom feed"
 msgstr "Flux web personnalisé"
 
-#: src/kerko/views/routes.py:120 src/kerko/views/searching.py:243
+#: src/kerko/views/routes.py:133 src/kerko/views/search.py:252
 msgid "Main feed"
 msgstr "Flux web principal"
 
-#: src/kerko/views/routes.py:229
+#: src/kerko/views/routes.py:242
 msgid ""
 "The document you have requested has been removed. Please check below for "
 "the latest documents available."
 msgstr ""
 "Le document demandé a été supprimé. Voyez ci-dessous pour les plus "
 "récents documents disponibles."
 
-#: src/kerko/views/searching.py:65
+#: src/kerko/views/search.py:66
 msgid "Your search did not match any resources"
 msgstr "Aucune ressource ne correspond à vos critères de recherche"
 
-#: src/kerko/views/searching.py:115 src/kerko/views/searching.py:191
-msgid "Full bibliography"
-msgstr "Bibliographie complète"
-
-#: src/kerko/views/searching.py:189
+#: src/kerko/views/search.py:198
 msgid "Result"
 msgid_plural "Results"
 msgstr[0] "Résultat"
 msgstr[1] "Résultats"
 
-#: src/kerko/views/searching.py:240
+#: src/kerko/views/search.py:249
 msgid "Custom feed based on your search"
 msgstr "Flux web personnalisé d’après vos critères de recherche"
```

### Comparing `Kerko-0.9/src/kerko/tree.py` & `Kerko-1.0.0a0/src/kerko/tree.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/views/breadbox.py` & `Kerko-1.0.0a0/src/kerko/views/breadbox.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/views/item_creators.py` & `Kerko-1.0.0a0/src/kerko/views/item/creators.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/views/item_facets.py` & `Kerko-1.0.0a0/src/kerko/views/item/facets.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/src/kerko/views/item_meta.py` & `Kerko-1.0.0a0/src/kerko/views/item/meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Utilities for preparing embedded metadata for HTML pages."""
 
 import re
 
 from flask import url_for
 
 from kerko.shortcuts import config
-from kerko.views.item_creators import format_creator_name
+from kerko.views.item.creators import format_creator_name
 
 
 def build_highwirepress_tags(item):  # pylint: disable=too-many-branches
     # References:
     # - https://scholar.google.ca/intl/en/scholar/inclusion.html#indexing
     # - https://www.monperrus.net/martin/accurate+bibliographic+metadata+and+google+scholar
     tags = []
     data = item.get('data', {})
-    if config('KERKO_HIGHWIREPRESS_TAGS') and data.get('itemType') in [
+    if config('kerko.meta.highwirepress_tags') and data.get('itemType') in [
         'book',
         'conferencePaper',
         'journalArticle',
         'report',
         'thesis',
     ]:
         tags.append(('citation_title', data.get('title', data.get('shortTitle', '')).strip()))
```

### Comparing `Kerko-0.9/src/kerko/views/item_relations.py` & `Kerko-1.0.0a0/src/kerko/views/item/relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,23 +45,23 @@
 def inject_relations(item):
     """
     Search and inject relations into the given item.
     """
     common_search_args = {
         'limit': None,
         'reject_any': {'item_type': ['note', 'attachment']},
-        'sort_spec': composer().sorts.get(config('KERKO_RELATIONS_SORT')),
+        'sort_spec': composer().sorts.get(config('kerko.features.relations_sort')),
         'faceting': False,
     }
     # For each related item, load the same fields as in normal search result
     # lists, except for the COinS field because we don't want it to get rendered
     # when displaying relations.
     related_item_fields = composer().select_fields(
         [
-            key for key in config('KERKO_RESULTS_FIELDS') +
+            key for key in config('kerko.search.result_fields') +
             [badge.field.key for badge in composer().badges.values()] if key != 'coins'
         ],
     )
     index = open_index('index')
     with Searcher(index) as searcher:
         for relation_spec in composer().relations.values():
             if relation_spec.directed:
```

### Comparing `Kerko-0.9/src/kerko/views/pager.py` & `Kerko-1.0.0a0/src/kerko/views/pager.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 def get_sections(page_num, page_count):
     """Return dict of pager sections, where each section is a list of page numbers."""
     if page_count <= 1:
         return None
 
     sections = {}
     page_num = min(max(page_num, 1), page_count)
-    first = max(1, int(page_num - config('KERKO_PAGER_LINKS') / 2))
-    last = min(page_count + 1, first + config('KERKO_PAGER_LINKS') + 1)
-    first = max(1, last - config('KERKO_PAGER_LINKS') - 1)
+    first = max(1, int(page_num - config('kerko.pagination.pager_links') / 2))
+    last = min(page_count + 1, first + config('kerko.pagination.pager_links') + 1)
+    first = max(1, last - config('kerko.pagination.pager_links') - 1)
 
     if page_num > 1:
         sections['first'] = [1]
         sections['previous'] = [max(1, page_num - 1)]
 
     sections['before'] = list(range(first, page_num))
     sections['current'] = [page_num]
```

### Comparing `Kerko-0.9/src/kerko/views/routes.py` & `Kerko-1.0.0a0/src/kerko/views/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,38 +3,35 @@
 from collections import deque
 from datetime import datetime, timedelta
 
 from flask import (abort, current_app, flash, make_response, redirect,
                    render_template, request, send_from_directory, url_for)
 from flask_babel import get_locale, gettext
 
-from kerko import babel_domain, blueprint
+from kerko import blueprint
 from kerko.criteria import create_feed_criteria, create_search_criteria
 from kerko.exceptions import except_abort
 from kerko.forms import SearchForm
 from kerko.searcher import Searcher
 from kerko.shortcuts import composer, config
 from kerko.specs import SortSpec
 from kerko.storage import (SchemaError, SearchIndexError, get_doc_count,
                            get_storage_dir, load_object, open_index)
-from kerko.views import (item_creators, item_facets, item_meta, item_relations,
-                         pager)
+from kerko.views import pager
+from kerko.views.item import build_item_context, creators, inject_item_data
 from kerko.views.search import search_list, search_single
 
 SITEMAP_URL_MAX_COUNT = 50000
 
 
 @blueprint.route('/', methods=['GET', 'POST'])
 @except_abort(SchemaError, 500)
 @except_abort(SearchIndexError, 503)
 def search():
     """View the results of a search."""
-    if config('KERKO_USE_TRANSLATIONS'):
-        babel_domain.as_default()
-
     criteria = create_search_criteria(request.args)
     form = SearchForm(csrf_enabled=False)
     if form.validate_on_submit():
         scope = composer().scopes.get(form.scope.data)
         if scope:
             # Add the newly submitted keywords, and redirect to search with them.
             url = url_for(
@@ -42,28 +39,26 @@
                 **criteria.params(
                     keywords=scope.add_keywords(form.keywords.data, criteria.keywords),
                     options={'page': None},
                 )
             )
             return redirect(url, 302)
 
-    if criteria.options.get('page-len', config('KERKO_PAGE_LEN')) == 1:
+    if criteria.options.get('page-len', config('kerko.pagination.page_len')) == 1:
         return search_single(criteria, form)
     return search_list(criteria, form)
 
 
 @blueprint.route('/atom.xml', methods=['GET'])
 @except_abort(SchemaError, 500)
 @except_abort(SearchIndexError, 503)
 def atom_feed():
     """Build a feed based on the search criteria."""
-    if config('KERKO_USE_TRANSLATIONS'):
-        babel_domain.as_default()
 
-    if 'atom' not in config('KERKO_FEEDS'):
+    if 'atom' not in config('kerko.feeds.formats'):
         return abort(404)
 
     context = {}
     criteria = create_feed_criteria(request.args)
     index = open_index('index')
     with Searcher(index) as searcher:
         extra_args = {}
@@ -78,46 +73,46 @@
             )
         else:
             current_app.logger.warning(
                 "Feed cannot be sorted because the 'sort_date_added' was "
                 "removed from the configuration."
             )
 
-        if config('KERKO_FEEDS_MAX_DAYS'):
+        if config('kerko.feeds.max_days'):
             if 'filter_date' in composer().fields:
                 today = datetime.today()
                 start = datetime(today.year, today.month,
-                                 today.day) - timedelta(config('KERKO_FEEDS_MAX_DAYS'))
+                                 today.day) - timedelta(config('kerko.feeds.max_days'))
                 current_app.logger.debug(
                     f"Show items dated {start} and newer"
-                    f" (KERKO_FEEDS_MAX_DAYS == {config('KERKO_FEEDS_MAX_DAYS')})."
+                    f" (kerko.feeds.max_days == {config('kerko.feeds.max_days')})."
                 )
                 extra_args['require_date_ranges'] = {'filter_date': (start, None)}
             else:
                 current_app.logger.warning(
-                    "'KERKO_FEEDS_MAX_DAYS' is set but has no effect because the "
+                    "'kerko.feeds.max_days' is set but has no effect because the "
                     "'filter_date' field was removed from the configuration."
                 )
 
         results = searcher.search_page(
             page=criteria.options.get('page', 1),
-            page_len=criteria.options.get('page-len', config('KERKO_PAGE_LEN')),
+            page_len=criteria.options.get('page-len', config('kerko.pagination.page_len')),
             keywords=criteria.keywords,
             filters=criteria.filters,
-            require_any=config('KERKO_FEEDS_REQUIRE_ANY'),  # Apply custom filtering, if not None.
-            reject_any={'item_type': ['note', 'attachment'], **config('KERKO_FEEDS_REJECT_ANY')},
+            require_any=config('kerko.feeds.require_any'),  # Apply custom filtering, if not None.
+            reject_any={'item_type': ['note', 'attachment'], **config('kerko.feeds.reject_any')},
             faceting=False,
             **extra_args,
         )
         if results.is_empty():
             items = []
         else:
-            items = results.items(composer().select_fields(config('KERKO_FEEDS_FIELDS')))
+            items = results.items(composer().select_fields(config('kerko.feeds.fields')))
             for item in items:
-                item_creators.inject_creator_display_names(item)
+                creators.inject_creator_display_names(item)
         context['items'] = items
         context['total_count'] = results.item_count
         criteria.fit_page(results.page_count or 1)
         pager_sections = pager.get_sections(criteria.options['page'], results.page_count or 1)
 
     last_sync = load_object('index', 'last_update_from_zotero')
     if last_sync:
@@ -130,19 +125,19 @@
     if criteria.is_searching():
         context['feed_title'] = gettext('Custom feed')
     else:
         context['feed_title'] = gettext('Main feed')
 
     response = make_response(
         render_template(
-            config('KERKO_TEMPLATE_ATOM_FEED'),
+            config('kerko.templates.atom_feed'),
             pager=pager.build_pager(
                 pager_sections, criteria, endpoint='kerko.atom_feed', _external=True
             ),
-            page_len=config('KERKO_PAGE_LEN'),
+            page_len=config('kerko.pagination.page_len'),
             feed_url=url_for(
                 '.atom_feed',
                 _external=True,
                 **criteria.params(
                     options={
                         'page': criteria.options['page'] if criteria.options['page'] > 1 else None
                     }
@@ -165,17 +160,14 @@
 @blueprint.route('/<path:item_id>')
 @except_abort(SchemaError, 500)
 @except_abort(SearchIndexError, 503)
 def item_view(item_id):
     """View a full bibliographic record."""
     start_time = time.process_time()
 
-    if config('KERKO_USE_TRANSLATIONS'):
-        babel_domain.as_default()
-
     index = open_index('index')
     with Searcher(index) as searcher:
         # Try matching the item by id, with fallback to alternate id.
         try_id_fields = deque(['id', 'alternate_id'])
         fellback = False
         while try_id_fields:
             results = searcher.search(
@@ -187,26 +179,20 @@
             if results.is_empty():
                 fellback = True  # Not found on first attempt.
                 continue
             break  # Found item, or no more id fields to try.
         if results.is_empty():
             return abort(404)
         item = results.items(composer().fields, composer().facets)[0]
-        item_url = url_for('.item_view', item_id=item['id'], _external=True)
         if fellback:
-            return redirect(item_url, 301)
-    item_creators.inject_creator_display_names(item)
-    item_relations.inject_relations(item)
-    item_facets.inject_facet_results(item)
+            return redirect(url_for('.item_view', item_id=item['id']), 301)
+    inject_item_data(item)
     return render_template(
-        config('KERKO_TEMPLATE_ITEM'),
-        item=item,
-        item_url=item_url,
-        title=item.get('data', {}).get('title', ''),
-        highwirepress_tags=item_meta.build_highwirepress_tags(item),
+        config('kerko.templates.item'),
+        **build_item_context(item),
         time=time.process_time() - start_time,
         locale=get_locale(),
     )
 
 
 @blueprint.route('/<path:item_id>/download/<string:attachment_id>/')
 @blueprint.route('/<path:item_id>/download/<string:attachment_id>/<string:attachment_filename>')
@@ -216,17 +202,14 @@
     """
     Download a child attachment.
 
     If the URL does not specify the attachment's filename or provides the wrong
     filename, a redirect is performed to a corrected URL so that the client gets
     a proper filename.
     """
-    if config('KERKO_USE_TRANSLATIONS'):
-        babel_domain.as_default()
-
     index = open_index('index')
     with Searcher(index) as searcher:
         # Try matching the item by id, with fallback to alternate id.
         try_id_fields = deque(['id', 'alternate_id'])
         fellback = False
         while try_id_fields:
             results = searcher.search(
@@ -465,11 +448,24 @@
             page_len=SITEMAP_URL_MAX_COUNT,
             reject_any={'item_type': ['note', 'attachment']},
             sort_spec=sort_spec,
             faceting=False,
         )
         if results.is_empty():
             return abort(404)
-        items = results.items(composer().select_fields(['id', 'z_dateModified']))
+        items = results.items(composer().select_fields(['id', 'date_modified']))
     response = make_response(render_template('kerko/sitemap.xml.jinja2', items=items))
     response.headers['Content-Type'] = 'application/xml; charset=utf-8'
     return response
+
+
+@blueprint.route('/api/last-sync')
+def last_updated_on():
+    last_sync = load_object('index', 'last_update_from_zotero')
+    if last_sync:
+        return {
+            'when': datetime.fromtimestamp(
+                last_sync, tz=datetime.now().astimezone().tzinfo
+            ).isoformat(),
+            'hours_ago': round((time.time() - last_sync) / 3600, 3),
+        }
+    return {}
```

### Comparing `Kerko-0.9/src/kerko/views/search.py` & `Kerko-1.0.0a0/src/kerko/views/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from flask_babel import get_locale, gettext, ngettext
 from werkzeug.datastructures import MultiDict
 
 from kerko.criteria import create_feed_criteria
 from kerko.searcher import Searcher
 from kerko.shortcuts import composer, config
 from kerko.storage import load_object, open_index
-from kerko.views import (breadbox, item_creators, item_facets, item_meta,
-                         item_relations, pager, sorter)
+from kerko.views import breadbox, pager, sorter
+from kerko.views.item import build_item_context, inject_item_data
 
 
 def _build_item_search_urls(items, criteria):
     """Generate an URL for each search result (switching the search to page-len=1)."""
     def build_url(item, position):
         return url_for(
             '.search',
@@ -24,15 +24,15 @@
                     'page': (criteria.options.get('page', 1) - 1) * page_len + position + 1,
                     'page-len': 1,
                     'id': item['id'],
                 }
             )
         )
 
-    page_len = criteria.options.get('page-len', config('KERKO_PAGE_LEN'))
+    page_len = criteria.options.get('page-len', config('kerko.pagination.page_len'))
     if page_len == 'all':
         page_len = 0
     return [build_url(item, position) for position, item in enumerate(items)]
 
 
 def _get_page_item_ids(criteria, page_numbers, current_item_id):
     """Retrieve the id of each item corresponding to the specified search result pages."""
@@ -79,15 +79,15 @@
                     reject_any={'item_type': ['note', 'attachment']},
                     limit=1,  # We don't care about the actual items.
                     faceting=True,
                 )
                 facets.update(results.facets(composer().facets, criteria, active_only=True))
     context['breadbox'] = breadbox.build_breadbox(criteria, facets)
     return render_template(
-        config('KERKO_TEMPLATE_SEARCH'),
+        config('kerko.templates.search'),
         form=form,
         locale=get_locale(),
         is_searching=criteria.is_searching(),
         **context,
     )
 
 
@@ -120,23 +120,17 @@
             context['search_title'] = gettext('Your search')
         else:
             context['search_title'] = gettext('Full bibliography')
 
         # Load item with all available fields.
         item = results.items(composer().fields, composer().facets)[0]
         facets = results.facets(composer().facets, criteria, active_only=True)
-        item_creators.inject_creator_display_names(item)
-        item_relations.inject_relations(item)
-        item_facets.inject_facet_results(item)
-
-        context['item'] = item
-        context['item_url'] = url_for('.item_view', item_id=item['id'], _external=True)
-        context['title'] = item.get('data', {}).get('title', '')
-        context['highwirepress_tags'] = item_meta.build_highwirepress_tags(item)
 
+        inject_item_data(item)
+        context.update(build_item_context(item))
         context['total_count'] = results.item_count
         context['total_count_formatted'] = format_decimal(results.item_count, locale=get_locale())
         context['page_count'] = results.page_count
         context['page_count_formatted'] = format_decimal(results.page_count, locale=get_locale())
         pager_sections = pager.get_sections(criteria.options['page'], results.page_count)
         page_item_ids = _get_page_item_ids(
             criteria, pager.get_page_numbers(pager_sections), item['id']
@@ -148,38 +142,38 @@
         )
         context['breadbox'] = breadbox.build_breadbox(criteria, facets)
         context['back_url'] = url_for(
             '.search',
             **criteria.params(
                 options={
                     'page': int(
-                        (criteria.options.get('page', 1) - 1) / config('KERKO_PAGE_LEN') + 1
+                        (criteria.options.get('page', 1) - 1) / config('kerko.pagination.page_len') + 1
                     ),
                     'page-len': None,
                     'id': None,
                 }
             )
         )
     return render_template(
-        config('KERKO_TEMPLATE_SEARCH_ITEM'),
+        config('kerko.templates.search_item'),
         form=form,
         time=time.process_time() - start_time,
         locale=get_locale(),
         is_searching=criteria.is_searching(),
         **context,
     )
 
 
 def search_list(criteria, form):
     """Perform search, and prepare the template context variables for a list of search results."""
     start_time = time.process_time()
     context = {}
     index = open_index('index')
     with Searcher(index) as searcher:
-        page_len = criteria.options.get('page-len', config('KERKO_PAGE_LEN'))
+        page_len = criteria.options.get('page-len', config('kerko.pagination.page_len'))
         common_search_args = {
             'keywords': criteria.keywords,
             'filters': criteria.filters,
             'reject_any': {'item_type': ['note', 'attachment']},
             'sort_spec': criteria.get_active_sort_spec(),
             'faceting': True,
         }
@@ -210,22 +204,22 @@
         context['page_count_formatted'] = format_decimal(results.page_count, locale=get_locale())
         context['pager'] = pager.build_pager(
             pager.get_sections(criteria.options['page'], results.page_count),
             criteria,
         )
         context['sorter'] = sorter.build_sorter(criteria)
         context['show_abstracts'] = criteria.options.get(
-            'abstracts', config('KERKO_RESULTS_ABSTRACTS')
+            'abstracts', config('kerko.features.results_abstracts')
         )
         context['abstracts_toggler_url'] = url_for(
             '.search',
             **criteria.params(options={
                 'abstracts': int(
                     not criteria.options.
-                    get('abstracts', config('KERKO_RESULTS_ABSTRACTS'))
+                    get('abstracts', config('kerko.features.results_abstracts'))
                 ),
             })
         )
         context['print_url'] = url_for(
             '.search',
             **criteria.params(options={
                 'page': None,
@@ -240,45 +234,45 @@
                 citation_format_key=key,
                 **criteria.params(options={
                     'page': None,
                 })
             )
             for key in composer().citation_formats.keys()
         }
-        if 'atom' in config('KERKO_FEEDS'):
+        if 'atom' in config('kerko.feeds.formats'):
             context['atom_feed_url'] = url_for(
                 '.atom_feed',
                 **create_feed_criteria(initial=criteria).params(options={
                     'page': None,
                 })
             )
             if criteria.is_searching():
                 context['atom_feed_help'] = gettext('Custom feed based on your search')
                 context['atom_feed_title'] = gettext('Custom feed')
             else:
                 context['atom_feed_title'] = gettext('Main feed')
 
         # Prepare search result items.
         field_specs = composer().select_fields(
-            config('KERKO_RESULTS_FIELDS') +
+            config('kerko.search.result_fields') +
             [badge.field.key for badge in composer().badges.values()],
         )
         items = results.items(field_specs)
-        facets = results.facets(composer().facets, criteria)
+        results_facets = results.facets(composer().facets, criteria)
         context['search_results'] = zip(items, _build_item_search_urls(items, criteria))
-        context['facet_results'] = facets
-        context['breadbox'] = breadbox.build_breadbox(criteria, facets)
+        context['facet_results'] = results_facets
+        context['breadbox'] = breadbox.build_breadbox(criteria, results_facets)
 
         last_sync = load_object('index', 'last_update_from_zotero')
         if last_sync:
             context['last_sync'] = datetime.fromtimestamp(
                 last_sync,
                 tz=datetime.now().astimezone().tzinfo,
             )
     return render_template(
-        config('KERKO_TEMPLATE_SEARCH'),
+        config('kerko.templates.search'),
         form=form,
         time=time.process_time() - start_time,
         locale=get_locale(),
         is_searching=criteria.is_searching(),
         **context,
     )
```

### Comparing `Kerko-0.9/src/kerko/views/sorter.py` & `Kerko-1.0.0a0/src/kerko/views/sorter.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/README.md` & `Kerko-1.0.0a0/tests/integration_testing/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ## Updating the saved responses
 
 - Before making any changes, make sure all the tests pass. If they don't pass
   after the changes, you will know that breaking changes happened either in the
   Zotero library's test data or in the way the Zotero API responded.
 - Go to the `api_responses` directory.
-- Set the `KERKO_ZOTERO_API_KEY` environment variable, or set it in a `.env`
+- Set the `ZOTERO_API_KEY` environment variable, or set it in a `.env`
   file in the `api_responses` directory.
 - Run the `update.bash` script from that directory to update the JSON files.
 - Note the values for the headers indicated below (which are output by
   `update.bash`), and update the corresponding variables in the
   `integration_testing` module, i.e.:
     - Total-Results → `ZOTERO_ITEMS_TOTAL_RESULTS`
     - Last-Modified-Version → `ZOTERO_ITEMS_LAST_MODIFIED_VERSION`
```

### Comparing `Kerko-0.9/tests/integration_testing/__init__.py` & `Kerko-1.0.0a0/tests/integration_testing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 import sys
 import tempfile
 import unittest
 
 import responses
 from flask import Flask, current_app
 from flask_babel import Babel, Domain
-from flask_bootstrap import Bootstrap
-from kerko import blueprint as kerko_blueprint
+from flask_bootstrap import Bootstrap4
+
+import kerko
 from kerko import extractors, transformers
 from kerko.composer import Composer
+from kerko.config_helpers import config_update, parse_config
 from kerko.storage import delete_storage
 from kerko.sync.cache import sync_cache
 from kerko.sync.index import sync_index
 
 
 class MockLibraryTestCase(unittest.TestCase):
     """Base test case providing mock Zotero API responses."""
 
     URL_PREFIX = '/bibliography'
 
     ZOTERO_RESPONSE_HEADERS = {
-        'Content-Type': 'application/json',
         'Zotero-API-Version': '3',
         'Zotero-Schema-Version': '15',
     }
 
     ZOTERO_ITEM_TYPES = [
         'artwork',
         'audioRecording',
@@ -76,37 +77,37 @@
     def get_response(response_name):
         response_path = pathlib.Path(__file__).parent / 'api_responses' / (response_name + '.json')
         with response_path.open() as f:
             return f.read()
 
     @classmethod
     def init_blueprints(cls):
-        cls.app.register_blueprint(kerko_blueprint, url_prefix=cls.URL_PREFIX)
+        cls.app.register_blueprint(kerko.blueprint, url_prefix=cls.URL_PREFIX)
 
     @classmethod
     def init_extensions(cls):
         cls._babel_domain = Domain()
         cls._babel = Babel(default_domain=cls._babel_domain)
         cls._babel.init_app(cls.app)
-        cls._bootstrap = Bootstrap()
+        cls._bootstrap = Bootstrap4()
         cls._bootstrap.init_app(cls.app)
 
     @classmethod
     def init_config(cls):
+        config_update(cls.app.config, kerko.DEFAULTS)
         cls.app.config['SECRET_KEY'] = 'not-so-secret-secret'
-        cls.app.config['KERKO_ZOTERO_API_KEY'] = 'xxxxxxxxxxxxxxxxxxxxxxxx'
-        cls.app.config['KERKO_ZOTERO_LIBRARY_ID'] = '9999999'
-        cls.app.config['KERKO_ZOTERO_LIBRARY_TYPE'] = 'group'
-        cls.app.config['KERKO_ZOTERO_MAX_ATTEMPTS'] = 1
-        cls.app.config['KERKO_ZOTERO_WAIT'] = 0
-        cls.app.config['KERKO_DATA_DIR'] = pathlib.Path(cls.temp_dir.name)
-        cls.app.config['KERKO_COMPOSER'] = Composer()
+        cls.app.config['ZOTERO_API_KEY'] = 'xxxxxxxxxxxxxxxxxxxxxxxx'
+        cls.app.config['ZOTERO_LIBRARY_ID'] = '9999999'
+        cls.app.config['ZOTERO_LIBRARY_TYPE'] = 'group'
+        cls.app.config['DATA_PATH'] = cls.temp_dir.name
+        parse_config(cls.app.config)
+        cls.app.config['kerko_composer'] = Composer(cls.app.config)
 
         # Add alternate_id to help retrieving and testing specific items.
-        cls.app.config['KERKO_COMPOSER'].fields['alternate_id'].extractor.extractors.append(
+        cls.app.config['kerko_composer'].fields['alternate_id'].extractor.extractors.append(
             extractors.TransformerExtractor(
                 extractor=extractors.ItemDataExtractor(key='extra'),
                 transformers=[
                     transformers.find(
                         regex=r'^\s*KerkoTestID\s*:\s*([0-9\-A-Z]+)\s*$',
                         flags=re.IGNORECASE | re.MULTILINE,
                         max_matches=1,
@@ -124,40 +125,39 @@
         regardless of the Zotero library.
 
         Subclasses should override this method to add more responses.
         """
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/itemTypes',
-            match_querystring=False,
-            content_type='application/json',
             body=cls.get_response('itemTypes'),
+            content_type='application/json',
             headers=cls.ZOTERO_RESPONSE_HEADERS,
         )
         for item_type in cls.ZOTERO_ITEM_TYPES:
             cls.responses.add(
                 responses.GET,
                 re.compile(
                     re.escape(
                         f'https://api.zotero.org/itemTypeFields?itemType={item_type}&locale=en-US'
                     ) + r'(\&timeout=[0-9]+)?'
                 ),
-                content_type='application/json',
                 body=cls.get_response(f'itemTypeFields_{item_type}'),
+                content_type='application/json',
                 headers=cls.ZOTERO_RESPONSE_HEADERS,
             )
             cls.responses.add(
                 responses.GET,
                 re.compile(
                     re.escape(
                         f'https://api.zotero.org/itemTypeCreatorTypes?itemType={item_type}&locale=en-US'
                     ) + r'(\&timeout=[0-9]+)?'
                 ),
-                content_type='application/json',
                 body=cls.get_response(f'itemTypeCreatorTypes_{item_type}'),
+                content_type='application/json',
                 headers=cls.ZOTERO_RESPONSE_HEADERS,
             )
 
     @classmethod
     def setUpClass(cls):
         """
         Prepare the test fixtures.
@@ -204,107 +204,107 @@
 
     @classmethod
     def add_responses(cls):
         super().add_responses()
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/collections?start=0&limit=100&format=json',
-            content_type='application/json',
             body=cls.get_response('collections'),
+            content_type='application/json',
             headers=cls.ZOTERO_RESPONSE_HEADERS,
         )
+        # Fallback for other 'collections' requests.
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/collections',
-            match_querystring=False,  # Fallback for other 'collections' requests.
-            content_type='application/json',
             body='[]',
+            content_type='application/json',
             headers=cls.ZOTERO_RESPONSE_HEADERS,
         )
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/items?since=0&start=0&limit=100&sort=dateAdded&direction=asc&include=bib%2Cbibtex%2Ccoins%2Cdata%2Cris&style=apa&format=json',
-            content_type='application/json',
             body=cls.get_response('items'),
+            content_type='application/json',
             headers={
                 **cls.ZOTERO_RESPONSE_HEADERS,
                 **{
                     'Total-Results': cls.ZOTERO_ITEMS_TOTAL_RESULTS,
                     'Last-Modified-Version': cls.ZOTERO_ITEMS_LAST_MODIFIED_VERSION,
                 }
             },
         )
         cls.responses.add(
             responses.GET,
             f'https://api.zotero.org/groups/9999999/items?since=0&start={cls.ZOTERO_ITEMS_TOTAL_RESULTS}&limit=100&sort=dateAdded&direction=asc&include=bib%2Cbibtex%2Ccoins%2Cdata%2Cris&style=apa&format=json',
-            content_type='application/json',
             body='[]',
+            content_type='application/json',
             headers={
                 **cls.ZOTERO_RESPONSE_HEADERS,
                 **{
                     'Total-Results': cls.ZOTERO_ITEMS_TOTAL_RESULTS,
                 }
             },
         )
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/items?limit=1&format=json',
-            content_type='application/json',
             body=cls.get_response('items_versions'),
+            content_type='application/json',
             headers={
                 **cls.ZOTERO_RESPONSE_HEADERS,
                 **{
                     'Total-Results': cls.ZOTERO_ITEMS_TOTAL_RESULTS,
                     'Last-Modified-Version': cls.ZOTERO_ITEMS_LAST_MODIFIED_VERSION,
                 }
             },
         )
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/fulltext?since=0',
-            content_type='application/json',
             body=cls.get_response('fulltext'),
+            content_type='application/json',
             headers=cls.ZOTERO_RESPONSE_HEADERS,
         )
 
 
 class EmptyLibraryTestCase(MockLibraryTestCase):
     """Test case providing mock Zotero API responses for an empty library."""
 
     @classmethod
     def add_responses(cls):
         super().add_responses()
+        # Response for all 'collections' requests.
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/collections',
-            match_querystring=False,  # Response for all 'collections' requests.
-            content_type='application/json',
             body='[]',  # No collections.
+            content_type='application/json',
             headers=cls.ZOTERO_RESPONSE_HEADERS,
         )
+        # Response for all 'items' requests.
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/items',
-            match_querystring=False,  # Response for all 'items' requests.
-            content_type='application/json',
             body='[]',  # No items.
+            content_type='application/json',
             headers={
                 **cls.ZOTERO_RESPONSE_HEADERS,
                 **{
                     'Total-Results': '0',
                     'Last-Modified-Version': '1',
                 }
             },
         )
+        # Response for all 'fulltext' requests.
         cls.responses.add(
             responses.GET,
             'https://api.zotero.org/groups/9999999/fulltext',
-            match_querystring=False,  # Response for all 'fulltext' requests.
-            content_type='application/json',
             body='{}',
+            content_type='application/json',
             headers=cls.ZOTERO_RESPONSE_HEADERS,
         )
 
 
 class SynchronizedTestCase(PopulatedLibraryTestCase):
     """
     Test case providing synchronized data from the integration testing library.
```

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/collections.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/collections.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_artwork.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_artwork.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_bill.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bill.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_blogPost.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_blogPost.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_book.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_book.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_bookSection.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bookSection.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_case.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_case.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_document.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_document.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_email.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_email.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_film.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_film.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_forumPost.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_forumPost.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_hearing.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_hearing.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_interview.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_interview.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_letter.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_letter.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_manuscript.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_manuscript.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_map.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_map.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_patent.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_patent.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_podcast.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_podcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_preprint.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_preprint.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_presentation.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_presentation.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_report.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_report.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_statute.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_statute.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_thesis.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_thesis.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypeFields_webpage.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_webpage.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/itemTypes.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypes.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/items.json` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/items.json`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/integration_testing/api_responses/update.bash` & `Kerko-1.0.0a0/tests/integration_testing/api_responses/update.bash`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 #
 # Generate JSON responses for a set of Zotero API URIs.
 
 if [[ -e .env ]]; then
     echo "Loading .env from current directory..."
     source .env
 fi
-if [[ -z ${KERKO_ZOTERO_API_KEY} ]]; then
-    >&2 echo "Variable KERKO_ZOTERO_API_KEY is missing."
+if [[ -z ${ZOTERO_API_KEY} ]]; then
+    >&2 echo "Variable ZOTERO_API_KEY is missing."
     exit 1
 fi
-if [[ -z ${KERKO_ZOTERO_LIBRARY_ID} ]]; then
-    KERKO_ZOTERO_LIBRARY_ID="4507457"
+if [[ -z ${ZOTERO_LIBRARY_ID} ]]; then
+    ZOTERO_LIBRARY_ID="4507457"
 fi
-if [[ -z ${KERKO_ZOTERO_LIBRARY_TYPE} ]]; then
-    KERKO_ZOTERO_LIBRARY_TYPE="group"
+if [[ -z ${ZOTERO_LIBRARY_TYPE} ]]; then
+    ZOTERO_LIBRARY_TYPE="group"
 fi
 
 options="--no-progress-meter --retry-connrefused --retry-delay 120 --retry 5"
-prefix="${KERKO_ZOTERO_LIBRARY_TYPE}s"
+prefix="${ZOTERO_LIBRARY_TYPE}s"
 declare -a item_types=(
     "artwork"
     "audioRecording"
     "bill"
     "blogPost"
     "book"
     "bookSection"
@@ -56,20 +56,20 @@
     "thesis"
     "videoRecording"
     "webpage"
 )
 
 # Show headers (for informational purpose only).
 echo -e "\nShowing Zotero API response headers..."
-curl --include "https://api.zotero.org/${prefix}/${KERKO_ZOTERO_LIBRARY_ID}/items?v=3&key=${KERKO_ZOTERO_API_KEY}&limit=1&format=versions"
+curl --include "https://api.zotero.org/${prefix}/${ZOTERO_LIBRARY_ID}/items?v=3&key=${ZOTERO_API_KEY}&limit=1&format=versions"
 
 # Update response files.
 echo -e "\n\nUpdating Zotero API responses' content..."
-curl ${options} "https://api.zotero.org/${prefix}/${KERKO_ZOTERO_LIBRARY_ID}/collections?v=3&key=${KERKO_ZOTERO_API_KEY}" -o "collections.json"
-curl ${options} "https://api.zotero.org/${prefix}/${KERKO_ZOTERO_LIBRARY_ID}/items?v=3&key=${KERKO_ZOTERO_API_KEY}&since=0&start=0&limit=100&sort=dateAdded&direction=asc&format=json&include=bib%2Cbibtex%2Ccoins%2Cris%2Cdata&style=apa" -o "items.json"
-curl ${options} "https://api.zotero.org/${prefix}/${KERKO_ZOTERO_LIBRARY_ID}/items?v=3&key=${KERKO_ZOTERO_API_KEY}&limit=1&format=versions" -o "items_versions.json"
-curl ${options} "https://api.zotero.org/${prefix}/${KERKO_ZOTERO_LIBRARY_ID}/fulltext?v=3&key=${KERKO_ZOTERO_API_KEY}&since=0" -o "fulltext.json"
-curl ${options} "https://api.zotero.org/itemTypes?v=3&key=${KERKO_ZOTERO_API_KEY}&locale=en-US" -o "itemTypes.json"
+curl ${options} "https://api.zotero.org/${prefix}/${ZOTERO_LIBRARY_ID}/collections?v=3&key=${ZOTERO_API_KEY}" -o "collections.json"
+curl ${options} "https://api.zotero.org/${prefix}/${ZOTERO_LIBRARY_ID}/items?v=3&key=${ZOTERO_API_KEY}&since=0&start=0&limit=100&sort=dateAdded&direction=asc&format=json&include=bib%2Cbibtex%2Ccoins%2Cris%2Cdata&style=apa" -o "items.json"
+curl ${options} "https://api.zotero.org/${prefix}/${ZOTERO_LIBRARY_ID}/items?v=3&key=${ZOTERO_API_KEY}&limit=1&format=versions" -o "items_versions.json"
+curl ${options} "https://api.zotero.org/${prefix}/${ZOTERO_LIBRARY_ID}/fulltext?v=3&key=${ZOTERO_API_KEY}&since=0" -o "fulltext.json"
+curl ${options} "https://api.zotero.org/itemTypes?v=3&key=${ZOTERO_API_KEY}&locale=en-US" -o "itemTypes.json"
 for item_type in "${item_types[@]}"; do
-    curl ${options} "https://api.zotero.org/itemTypeFields?v=3&key=${KERKO_ZOTERO_API_KEY}&itemType=${item_type}" -o "itemTypeFields_${item_type}.json"
-    curl ${options} "https://api.zotero.org/itemTypeCreatorTypes?v=3&key=${KERKO_ZOTERO_API_KEY}&itemType=${item_type}" -o "itemTypeCreatorTypes_${item_type}.json"
+    curl ${options} "https://api.zotero.org/itemTypeFields?v=3&key=${ZOTERO_API_KEY}&itemType=${item_type}" -o "itemTypeFields_${item_type}.json"
+    curl ${options} "https://api.zotero.org/itemTypeCreatorTypes?v=3&key=${ZOTERO_API_KEY}&itemType=${item_type}" -o "itemTypeCreatorTypes_${item_type}.json"
 done
```

### Comparing `Kerko-0.9/tests/test_atom_feed.py` & `Kerko-1.0.0a0/tests/test_atom_feed.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     _external=True,
                     **create_feed_criteria().params(options={'page': None}),
                 ),
                 "feed.id is invalid",
             )
             self.assertRegex(
                 root.xpath('/ns:feed/ns:title/text()', namespaces=self.namespaces)[0],
-                rf'^{re.escape(config("KERKO_TITLE"))}',
+                rf'^{re.escape(config("kerko.meta.title"))}',
                 "feed.title is incorrect",
             )
             # Check date, with a compromise: not trying full ISO 8601 variants.
             self.assertIsInstance(
                 datetime.strptime(
                     root.xpath('/ns:feed/ns:updated/text()', namespaces=self.namespaces)[0][0:13],
                     '%Y-%m-%dT%H',
@@ -190,15 +190,15 @@
                         initial=MultiDict({'all': ['qwertyasdfghzxcvbn']})
                     ).params(options={'page': None}),
                 ),
                 "feed.id is missing or incorrect",
             )
             self.assertRegex(
                 root.xpath('/ns:feed/ns:title/text()', namespaces=self.namespaces)[0],
-                rf'^{re.escape(config("KERKO_TITLE"))}',
+                rf'^{re.escape(config("kerko.meta.title"))}',
                 "feed.title is missing or incorrect",
             )
             self.assertIsInstance(
                 datetime.strptime(
                     root.xpath('/ns:feed/ns:updated/text()', namespaces=self.namespaces)[0][0:13],
                     '%Y-%m-%dT%H',  # A compromise: not trying all ISO 8601 variants.
                 ),
```

### Comparing `Kerko-0.9/tests/test_datetime.py` & `Kerko-1.0.0a0/tests/test_datetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Unit tests for the datetime module.
 """
 
 import unittest
 from datetime import datetime
 
 from flask import Flask, current_app
-from flask_babel import Babel, Domain
+from flask_babel import Babel
 
-from kerko import blueprint as kerko_blueprint
+import kerko
 from kerko.datetime import (iso_to_datetime, maximize_partial_date,
                             parse_partial_date, reformat_date)
 
 
 class ParsePartialDateTestCase(unittest.TestCase):
     """Test the `parse_partial_date()` function."""
 
@@ -152,24 +152,23 @@
 
 
 class DateStringReformattingTestCase(unittest.TestCase):
     """Test the date string reformatting function."""
 
     def setUp(self):
         self.app = Flask(__name__)
-        self.app.register_blueprint(kerko_blueprint, url_prefix='/bibliography')
-        babel_domain = Domain()
-        babel = Babel(default_domain=babel_domain)
-        babel.init_app(self.app)
+        self.app.register_blueprint(kerko.blueprint, url_prefix='/bibliography')
+        self.babel = Babel()
         ctx = self.app.app_context()
         ctx.push()
 
     def test_non_iso8601_utc_en(self):
         current_app.config['BABEL_DEFAULT_LOCALE'] = 'en_US'
         current_app.config['BABEL_DEFAULT_TIMEZONE'] = 'UTC'
+        self.babel.init_app(current_app)
         self.assertEqual(reformat_date('2020'), '2020')
         self.assertEqual(reformat_date('2020-10'), '2020-10')
         self.assertEqual(reformat_date('2020-05-05'), '2020-05-05')
         self.assertEqual(reformat_date('01/02/2021'), '01/02/2021')
         self.assertEqual(reformat_date('September 2020'), 'September 2020')
         self.assertEqual(reformat_date('September 20, 2020'), 'September 20, 2020')
         self.assertEqual(
@@ -179,124 +178,128 @@
             reformat_date('September 20, 2020', convert_tz=True, show_tz=True),
             'September 20, 2020'
         )
 
     def test_iso8601_utc_en(self):
         current_app.config['BABEL_DEFAULT_LOCALE'] = 'en_US'
         current_app.config['BABEL_DEFAULT_TIMEZONE'] = 'UTC'
-        self.assertEqual(
+        self.babel.init_app(current_app)
+        self.assertRegex(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=True),
-            '9/17/20, 7:11 AM'
+            r'9/17/20, 7:11\sAM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=False),
-            '9/17/20, 7:11 AM'
+            r'9/17/20, 7:11\sAM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=True, show_tz=True),
-            '9/17/20, 7:11 AM (UTC)'
+            r'9/17/20, 7:11\sAM\s\(UTC\)'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19Z', convert_tz=True),
-            '11/7/20, 12:30 PM'
+            r'11/7/20, 12:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19Z', convert_tz=False),
-            '11/7/20, 12:30 PM'
+            r'11/7/20, 12:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19Z', convert_tz=True, show_tz=True),
-            '11/7/20, 12:30 PM (UTC)'
+            r'11/7/20, 12:30\sPM\s\(UTC\)'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2019-07-22T20:42+00:00', convert_tz=True),
-            '7/22/19, 8:42 PM'
+            r'7/22/19, 8:42\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2019-07-22T20:42+00:00', convert_tz=False),
-            '7/22/19, 8:42 PM'
+            r'7/22/19, 8:42\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2019-07-22T20:42+00:00', convert_tz=True, show_tz=True),
-            '7/22/19, 8:42 PM (UTC)'
+            r'7/22/19, 8:42\sPM\s\(UTC\)'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19-0500', convert_tz=True),
-            '11/7/20, 5:30 PM'
+            r'11/7/20, 5:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19-0500', convert_tz=False),
-            '11/7/20, 12:30 PM'
+            r'11/7/20, 12:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19-0500', convert_tz=True, show_tz=True),
-            '11/7/20, 5:30 PM (UTC)'
+            r'11/7/20, 5:30\sPM\s\(UTC\)'
         )
 
     def test_iso8601_est_en(self):
         current_app.config['BABEL_DEFAULT_LOCALE'] = 'en_US'
         current_app.config['BABEL_DEFAULT_TIMEZONE'] = 'EST'
-        self.assertEqual(
+        self.babel.init_app(current_app)
+        self.assertRegex(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=True),
-            '9/17/20, 2:11 AM'
+            r'9/17/20, 2:11\sAM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=False),
-            '9/17/20, 7:11 AM'
+            r'9/17/20, 7:11\sAM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=True, show_tz=True),
-            '9/17/20, 2:11 AM (EST)'
+            r'9/17/20, 2:11\sAM\s\(EST\)'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19Z', convert_tz=True),
-            '11/7/20, 7:30 AM'
+            r'11/7/20, 7:30\sAM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19Z', convert_tz=False),
-            '11/7/20, 12:30 PM'
+            r'11/7/20, 12:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19Z', convert_tz=True, show_tz=True),
-            '11/7/20, 7:30 AM (EST)'
+            r'11/7/20, 7:30\sAM\s\(EST\)'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2019-07-22T20:42+00:00', convert_tz=True),
-            '7/22/19, 3:42 PM'
+            r'7/22/19, 3:42\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2019-07-22T20:42+00:00', convert_tz=False),
-            '7/22/19, 8:42 PM'
+            r'7/22/19, 8:42\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2019-07-22T20:42+00:00', convert_tz=True, show_tz=True),
-            '7/22/19, 3:42 PM (EST)'
+            r'7/22/19, 3:42\sPM\s\(EST\)'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19-0500', convert_tz=True),
-            '11/7/20, 12:30 PM'
+            r'11/7/20, 12:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19-0500', convert_tz=False),
-            '11/7/20, 12:30 PM'
+            r'11/7/20, 12:30\sPM'
         )
-        self.assertEqual(
+        self.assertRegex(
             reformat_date('2020-11-07T12:30:19-0500', convert_tz=True, show_tz=True),
-            '11/7/20, 12:30 PM (EST)'
+            r'11/7/20, 12:30\sPM\s\(EST\)'
         )
 
     def test_non_iso8601_utc_fr(self):
         current_app.config['BABEL_DEFAULT_LOCALE'] = 'fr_FR'
         current_app.config['BABEL_DEFAULT_TIMEZONE'] = 'UTC'
+        self.babel.init_app(current_app)
         self.assertEqual(reformat_date('September 2020'), 'September 2020')
         self.assertEqual(reformat_date('September 20, 2020'), 'September 20, 2020')
 
     def test_iso8601_utc_fr(self):
         current_app.config['BABEL_DEFAULT_LOCALE'] = 'fr_FR'
         current_app.config['BABEL_DEFAULT_TIMEZONE'] = 'UTC'
+        self.babel.init_app(current_app)
         self.assertEqual(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=True),
             '17/09/2020 07:11'
         )
         self.assertEqual(
             reformat_date('2020-09-17T07:11:41+00:00', convert_tz=False),
             '17/09/2020 07:11'
```

### Comparing `Kerko-0.9/tests/test_item_meta.py` & `Kerko-1.0.0a0/tests/test_item_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Tests for item meta tags.
 """
 
 import unittest
 
 import elementpath  # For XPath 2.0 selectors.
 from lxml import etree
-from kerko.views.item_creators import format_creator_name
+from kerko.views.item.creators import format_creator_name
 
 from tests.integration_testing import SynchronizedTestCase
 
 
 class CreatorNameTestCase(unittest.TestCase):
     """Unit test for creator name formatting."""
```

### Comparing `Kerko-0.9/tests/test_pager.py` & `Kerko-1.0.0a0/tests/test_pager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """
 Unit tests for the pager module.
 """
 
 import unittest
 
-from flask import current_app, Flask
+from flask import Flask
 
-from kerko import blueprint as kerko_blueprint
+import kerko
+from kerko.config_helpers import config_update
+from kerko.shortcuts import config
 from kerko.views import pager
 
 
 class SectionsTestCase(unittest.TestCase):
     """Test pager sections when there is a single page."""
 
     def setUp(self):
         self.app = Flask(__name__)
-        self.app.register_blueprint(kerko_blueprint, url_prefix='/bibliography')
+        config_update(self.app.config, kerko.DEFAULTS)
+        self.app.register_blueprint(kerko.blueprint, url_prefix='/bibliography')
         ctx = self.app.app_context()
         ctx.push()
 
     def test_default_config(self):
         # This setting impacts the results of pager functions.
-        self.assertEqual(current_app.config['KERKO_PAGER_LINKS'], 4)
+        self.assertEqual(config('kerko.pagination.pager_links'), 4)
 
     def test_on_page_1_of_1(self):
         sections = pager.get_sections(page_num=1, page_count=1)
         self.assertIsNone(sections)
         pages = pager.get_page_numbers(sections)
         self.assertFalse(pages)
```

### Comparing `Kerko-0.9/tests/test_sitemap.py` & `Kerko-1.0.0a0/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tests/test_sync.py` & `Kerko-1.0.0a0/tests/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     """
 
     def test_sync_library_context(self):
         zotero_credentials = zotero.init_zotero()
         library_context = zotero.request_library_context(zotero_credentials)
         self.assertEqual(
             library_context.library_id,
-            current_app.config['KERKO_ZOTERO_LIBRARY_ID'],
+            current_app.config['ZOTERO_LIBRARY_ID'],
         )
         self.assertEqual(
             library_context.library_type,
-            current_app.config['KERKO_ZOTERO_LIBRARY_TYPE'],
+            current_app.config['ZOTERO_LIBRARY_TYPE'],
         )
         self.assertEqual(set(library_context.item_types.keys()), set(self.ZOTERO_ITEM_TYPES))
         self.assertEqual(set(library_context.item_fields.keys()), set(self.ZOTERO_ITEM_TYPES))
         self.assertEqual(set(library_context.creator_types.keys()), set(self.ZOTERO_ITEM_TYPES))
         # TODO: Assert more things.
 
     def test_sync_index(self):
```

### Comparing `Kerko-0.9/tests/test_tags.py` & `Kerko-1.0.0a0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `Kerko-0.9/tox.ini` & `Kerko-1.0.0a0/tox.ini`

 * *Files identical despite different names*

