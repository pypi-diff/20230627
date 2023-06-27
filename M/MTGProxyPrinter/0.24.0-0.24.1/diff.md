# Comparing `tmp/MTGProxyPrinter-0.24.0.tar.gz` & `tmp/MTGProxyPrinter-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MTGProxyPrinter-0.24.0.tar", last modified: Mon Jun 26 12:25:24 2023, max compression
+gzip compressed data, was "MTGProxyPrinter-0.24.1.tar", last modified: Tue Jun 27 15:48:00 2023, max compression
```

## Comparing `MTGProxyPrinter-0.24.0.tar` & `MTGProxyPrinter-0.24.1.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/LICENSE.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.24.0/MANIFEST.in
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13399 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      224 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8781 2023-06-26 12:16:57.000000 MTGProxyPrinter-0.24.0/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2023-06-08 13:24:21.000000 MTGProxyPrinter-0.24.0/ThirdPartyLicenses.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/doc/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    43567 2023-06-26 12:18:31.000000 MTGProxyPrinter-0.24.0/doc/changelog.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3255 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/__main__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1437 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/app_dirs.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/application.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/argument_parser.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    34320 2023-06-08 15:23:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/card_info_downloader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16632 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_downloader.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/re_parsers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/_interface.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11404 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/card_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/compact_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/edit_document_settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/import_deck_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/load_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/move_cards.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/new_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/page_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/replace_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/shuffle_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/downloader_base.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/http_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2726 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/logger.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-06-26 12:19:05.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/meta_data.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/metered_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/missing_images_manager.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11186 2023-06-08 16:06:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/card_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    46173 2023-06-25 19:44:33.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8066 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    32805 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb_migrations.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v2.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v3.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v4.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v5.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2023-05-03 12:03:13.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v6.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    24082 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    26031 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_loader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1685 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    19124 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/imagedb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/string_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/natsort.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/print.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2175 2023-05-24 09:56:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/progress_meter.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.310116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      490 2023-05-06 09:19:50.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.310116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      441 2023-05-06 09:19:50.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2023-05-24 12:10:19.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2023-05-24 12:09:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2023-05-24 11:50:42.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      475 2023-05-24 11:50:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/index.theme
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7302 2023-05-24 12:15:01.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/resources.qrc
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/about_dialog.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4226 2023-05-24 13:03:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4081 2023-05-24 13:04:02.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3703 2023-05-24 13:04:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5018 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20314 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/main_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10340 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17043 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8583 2023-06-05 16:19:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/sqlite_helpers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/stop_thread.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/add_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21267 2023-06-08 13:21:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14318 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/central_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    31709 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/deck_import_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11677 2023-06-26 08:34:03.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/dialogs.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/about_dialog.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5497 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5224 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4125 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6843 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17319 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_dialog.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_widget.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13804 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3670 2023-06-08 16:06:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/item_delegates.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    26406 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_config_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    24943 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_renderer.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5903 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/printing_filter_widgets.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17242 2023-05-23 17:35:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3913 2023-06-26 08:32:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/units_and_sizes.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/update_checker.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5835 2023-06-26 11:58:49.000000 MTGProxyPrinter-0.24.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/LICENSE.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.24.1/MANIFEST.in
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13399 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      224 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8781 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/README.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/ThirdPartyLicenses.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/doc/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    44070 2023-06-27 15:46:22.000000 MTGProxyPrinter-0.24.1/doc/changelog.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3255 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/__main__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1437 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/app_dirs.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/application.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/argument_parser.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    34320 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/card_info_downloader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16632 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_downloader.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/csv_parsers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/re_parsers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/_interface.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11404 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/card_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/compact_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/edit_document_settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/import_deck_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/load_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/move_cards.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/new_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/page_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/replace_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/shuffle_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/downloader_base.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/http_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2726 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/logger.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-06-27 15:47:02.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/meta_data.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/metered_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/missing_images_manager.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11180 2023-06-27 15:32:36.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/card_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    46173 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8066 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    32805 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb_migrations.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v2.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v3.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v4.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v5.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2023-05-03 12:03:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v6.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    24223 2023-06-27 15:32:36.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    26031 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_loader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1685 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    19124 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/imagedb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/string_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/natsort.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/print.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2175 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/progress_meter.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.053226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.053226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      490 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.065227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      441 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.065227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/index.theme
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.053226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7302 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/resources.qrc
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/about_dialog.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4226 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4081 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3703 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5018 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20314 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/main_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_dialog.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_widget.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10340 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17043 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8583 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/sqlite_helpers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/stop_thread.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/add_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21267 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/cache_cleanup_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14900 2023-06-27 15:34:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/central_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    31709 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/deck_import_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11677 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/dialogs.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/about_dialog.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5497 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/columnar.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5224 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/grouped.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4125 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6843 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17319 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_dialog.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_widget.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13804 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3670 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/item_delegates.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    26406 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_config_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    24943 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_renderer.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5903 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/printing_filter_widgets.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17242 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3913 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/units_and_sizes.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/update_checker.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5835 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/setup.py
```

### Comparing `MTGProxyPrinter-0.24.0/LICENSE.md` & `MTGProxyPrinter-0.24.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/PKG-INFO` & `MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.24.0
+Version: 0.24.1
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/SOURCES.txt` & `MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/PKG-INFO` & `MTGProxyPrinter-0.24.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.24.0
+Version: 0.24.1
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MTGProxyPrinter-0.24.0/README.md` & `MTGProxyPrinter-0.24.1/README.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/ThirdPartyLicenses.md` & `MTGProxyPrinter-0.24.1/ThirdPartyLicenses.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/doc/changelog.md` & `MTGProxyPrinter-0.24.1/doc/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+# Version 0.24.1 (2023-06-27)  <a name="v0_24_1"></a>
+
+## Fixed issues
+
+- Fixed broken check card generation and addition of related cards. Both features failed to fetch the required images,
+  rendering the cards as white rectangles, instead of the expected card images.
+- Fixed display of the 5th column in the table showing the cards on the current page. It shows whether the image is
+  a front or back side of a (double-faced) card. It now has a proper header ("Side") and human-readable content.  
+
 # Version 0.24.0 (2023-06-26)  <a name="v0_24_0"></a>
 
 ## New features
 
 - Added basic support for printing custom cards. You can drag & drop image files onto the application window,
   which are then added to the document as regular-sized cards
     - Importing most common image formats is supported
```

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/__init__.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/__main__.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/__main__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/app_dirs.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/app_dirs.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/application.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/application.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/argument_parser.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/argument_parser.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/card_info_downloader.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/card_info_downloader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_downloader.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_downloader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/common.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/csv_parsers.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/csv_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/re_parsers.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/re_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/_interface.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/_interface.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/card_actions.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/card_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/compact_document.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/compact_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/edit_document_settings.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/edit_document_settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/import_deck_list.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/import_deck_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/load_document.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/load_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/move_cards.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/move_cards.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/new_document.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/new_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/page_actions.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/page_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/replace_card.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/replace_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/shuffle_document.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/shuffle_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/downloader_base.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/downloader_base.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/http_file.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/http_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/logger.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/logger.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/meta_data.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/meta_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 PROGRAMNAME = "MTGProxyPrinter"
-__version__ = "0.24.0"
+__version__ = "0.24.1"
 COPYRIGHT = "(C) 2019-2023 Thomas Hess"
 HOME_PAGE = "https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter"
 
 DOWNLOAD_WEB_PAGE = f"{HOME_PAGE}/uv/download.html"
 USER_AGENT = f"{PROGRAMNAME}/{__version__} ({HOME_PAGE})"
```

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/metered_file.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/metered_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/missing_images_manager.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/missing_images_manager.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/card_list.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/card_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
 
     header = {
         PageColumns.CardName: "Card name",
         PageColumns.Set: "Set",
         PageColumns.CollectorNumber: "Collector #",
         PageColumns.Language: "Language",
-        PageColumns.IsFront: "Front/Back",
+        PageColumns.IsFront: "Side",
     }
     EDITABLE_COLUMNS = {PageColumns.Set, PageColumns.CollectorNumber}
 
     oversized_card_count_changed = Signal(int)
 
     def __init__(self, card_db: CardDatabase, *args, **kwargs):
         super(CardListModel, self).__init__(*args, **kwargs)
```

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.sql` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb_migrations.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb_migrations.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v2.sql` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v2.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v3.sql` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v3.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v4.sql` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v4.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v5.sql` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v5.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v6.sql` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v6.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
     page_header = {
         PageColumns.CardName: "Card name",
         PageColumns.Set: "Set",
         PageColumns.CollectorNumber: "Collector #",
         PageColumns.Language: "Language",
         PageColumns.Image: "Image",
+        PageColumns.IsFront: "Side",
     }
     EDITABLE_COLUMNS = {PageColumns.Set, PageColumns.CollectorNumber}
 
     def __init__(self, card_db: CardDatabase, image_db: ImageDatabase, *args, **kwargs):
         super(Document, self).__init__(*args, **kwargs)
         self.undo_stack: ActionStack = collections.deque()
         self.redo_stack: ActionStack = collections.deque()
@@ -268,15 +269,17 @@
             elif index.column() == PageColumns.CollectorNumber:
                 return card.collector_number
             elif index.column() == PageColumns.Language:
                 return card.language
             elif index.column() == PageColumns.Image:
                 return card.image_file
             elif index.column() == PageColumns.IsFront:
-                return card.is_front
+                if role == Qt.EditRole:
+                    return card.is_front
+                return "Front" if card.is_front else "Back"
 
     @staticmethod
     def _get_page_preview(page: Page):
         names = collections.Counter(container.card.name for container in page)
         return "\n".join(
             f"{count}× {name}" for name, count in names.items()
         )
```

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_loader.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_loader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/imagedb.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/imagedb.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/string_list.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/string_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/natsort.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/natsort.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/print.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/print.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/progress_meter.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/progress_meter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/index.theme` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/index.theme`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/resources.qrc` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/about_dialog.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/columnar.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/grouped.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/main_window.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_dialog.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_widget.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_widget.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/settings.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/sqlite_helpers.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/sqlite_helpers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/stop_thread.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/stop_thread.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/add_card.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/add_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/cache_cleanup_wizard.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/central_widget.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/central_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,20 +167,29 @@
         card_name = card.name if isinstance(card, (Card, CheckCard)) else nl + nl.join(item.name for item in card)
         if count is None:
             count, success = QInputDialog.getInt(self, "Add copies", f"Add copies of {card_name}", 1, 1, 100)
             if not success:
                 logger.info("User cancelled adding card copies")
                 return
         logger.info(f"Add {count} × {card_name.replace(nl, ',')} via the context menu action")
-
         if isinstance(card, (Card, CheckCard)):
-            self.request_action.emit(ActionAddCard(card, count))
+            self._request_action_add_card(card, count)
         else:
             for item in card:
-                self.request_action.emit(ActionAddCard(item, count))
+                self._request_action_add_card(item, count)
+
+    def _request_action_add_card(self, card: typing.Union[Card, CheckCard], count: int):
+        # If cards have images, request the action directly. This happens when adding copies of already added cards
+        # and is required for custom cards. Otherwise, request the image from the image database. Cards without images
+        # at this point are CheckCards or related cards.
+        action = ActionAddCard(card, count)
+        if card.image_file is None:
+            self.obtain_card_image.emit(action)
+        else:
+            self.request_action.emit(action)
 
     def _add_save_image_action(self, parent: QMenu, card: typing.Union[Card, CheckCard]):
         action = QAction(QIcon.fromTheme("document-save"), "Export image", parent)
         action.setData(card)
         action.triggered.connect(self._on_save_image_action_triggered)
         parent.addSeparator()
         parent.addAction(action)
@@ -224,18 +233,20 @@
         self.ui.page_card_table_view.clearSelection()
         self.ui.page_card_table_view.setRootIndex(new_page.sibling(new_page.row(), new_page.column()))
         self.ui.page_card_table_view.setColumnHidden(PageColumns.Image, True)
         # The size adjustments have to be done here,
         # because the width can only be set after the model root index to show has been set
         default_column_width = 102
         for column, scaling_factor in (
-                (PageColumns.CardName, 1.7),
-                (PageColumns.Set, 2),
-                (PageColumns.CollectorNumber, 0.95),
-                (PageColumns.Language, 0.8)):
+            (PageColumns.CardName, 1.7),
+            (PageColumns.Set, 2),
+            (PageColumns.CollectorNumber, 0.95),
+            (PageColumns.Language, 0.8),
+            (PageColumns.IsFront, 0.8),
+        ):
             new_size = math.floor(default_column_width * scaling_factor)
             self.ui.page_card_table_view.setColumnWidth(column, new_size)
 
     def on_document_rows_about_to_be_removed(self, parent: QModelIndex, first: int, last: int):
         currently_selected_page = self.ui.document_view.currentIndex().row()
         is_page_index = not parent.isValid()
         if not is_page_index:
```

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/common.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/deck_import_wizard.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/deck_import_wizard.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/dialogs.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/about_dialog.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/about_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/columnar.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/grouped.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/main_window.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/main_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_dialog.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_widget.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/settings_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/item_delegates.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/item_delegates.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/main_window.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_config_widget.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_renderer.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_renderer.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/printing_filter_widgets.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/printing_filter_widgets.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/settings_window.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/settings_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/units_and_sizes.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/units_and_sizes.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/mtg_proxy_printer/update_checker.py` & `MTGProxyPrinter-0.24.1/mtg_proxy_printer/update_checker.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/pyproject.toml` & `MTGProxyPrinter-0.24.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.0/setup.py` & `MTGProxyPrinter-0.24.1/setup.py`

 * *Files identical despite different names*

