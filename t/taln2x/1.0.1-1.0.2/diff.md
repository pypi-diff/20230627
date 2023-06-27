# Comparing `tmp/taln2x-1.0.1.tar.gz` & `tmp/taln2x-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taln2x-1.0.1.tar", last modified: Fri Jun 23 14:00:31 2023, max compression
+gzip compressed data, was "taln2x-1.0.2.tar", last modified: Tue Jun 27 15:07:16 2023, max compression
```

## Comparing `taln2x-1.0.1.tar` & `taln2x-1.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.932493 taln2x-1.0.1/
--rw-rw-r--   0 yparment  (1000) yparment  (1000)       65 2023-02-16 14:40:42.000000 taln2x-1.0.1/.gitignore
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    35132 2023-02-06 10:46:05.000000 taln2x-1.0.1/LICENCE
--rw-rw-r--   0 yparment  (1000) yparment  (1000)       31 2023-06-23 13:55:10.000000 taln2x-1.0.1/MANIFEST.in
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     3107 2023-06-23 14:00:31.932493 taln2x-1.0.1/PKG-INFO
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     2388 2023-02-06 10:46:05.000000 taln2x-1.0.1/README.md
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1264 2023-06-08 07:15:42.000000 taln2x-1.0.1/pyproject.toml
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      137 2023-02-06 10:46:05.000000 taln2x-1.0.1/requirements.txt
--rw-rw-r--   0 yparment  (1000) yparment  (1000)       38 2023-06-23 14:00:31.932493 taln2x-1.0.1/setup.cfg
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.904492 taln2x-1.0.1/src/
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.908492 taln2x-1.0.1/src/taln2x/
--rw-rw-r--   0 yparment  (1000) yparment  (1000)       54 2023-06-23 14:00:10.000000 taln2x-1.0.1/src/taln2x/__init__.py
--rwxrwxr-x   0 yparment  (1000) yparment  (1000)    20234 2023-06-15 07:48:27.000000 taln2x-1.0.1/src/taln2x/__main__.py
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.912492 taln2x-1.0.1/src/taln2x/exports/
--rw-rw-r--   0 yparment  (1000) yparment  (1000)       53 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/exports/__init__.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    15746 2023-06-15 11:55:11.000000 taln2x-1.0.1/src/taln2x/exports/anthology.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    14434 2023-06-20 07:52:12.000000 taln2x-1.0.1/src/taln2x/exports/archives.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     6215 2023-06-15 13:35:06.000000 taln2x-1.0.1/src/taln2x/exports/dblp.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    27591 2023-06-19 12:07:51.000000 taln2x-1.0.1/src/taln2x/exports/hal.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    15264 2023-06-15 11:54:58.000000 taln2x-1.0.1/src/taln2x/exports/pdf.py
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.932493 taln2x-1.0.1/src/taln2x/templates/
--rw-rw-r--   0 yparment  (1000) yparment  (1000)  3321771 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/PDFBox-0.7.3.jar
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    35605 2023-06-19 09:22:47.000000 taln2x-1.0.1/src/taln2x/templates/aofr.xsd
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      923 2023-02-16 15:02:01.000000 taln2x-1.0.1/src/taln2x/templates/articles.csv
--rw-rw-r--   0 yparment  (1000) yparment  (1000)  2280976 2023-02-16 15:07:58.000000 taln2x-1.0.1/src/taln2x/templates/articles.zip
--rw-rw-r--   0 yparment  (1000) yparment  (1000)  3223045 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/background.png
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      701 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/blank.pdf
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    59921 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/by.eps
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     2275 2023-02-17 16:26:28.000000 taln2x-1.0.1/src/taln2x/templates/config.toml
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1428 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/dblpsubmission.dtd
--rwxrwxr-x   0 yparment  (1000) yparment  (1000)     9346 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/easy2acl.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      555 2023-02-16 15:05:52.000000 taln2x-1.0.1/src/taln2x/templates/event.yml
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     7921 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/logo.png
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     7626 2023-02-14 11:05:32.000000 taln2x-1.0.1/src/taln2x/templates/pre-proceedings-en.tex
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     7672 2023-02-14 12:23:42.000000 taln2x-1.0.1/src/taln2x/templates/pre-proceedings.tex
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     3704 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/templates/single_paper.tex
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     6408 2023-02-14 16:39:55.000000 taln2x-1.0.1/src/taln2x/templates/taln-archives.xsd
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.932493 taln2x-1.0.1/src/taln2x/utils/
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1014 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/utils/Article.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      591 2023-06-15 11:52:42.000000 taln2x-1.0.1/src/taln2x/utils/Author.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1469 2023-06-16 15:05:19.000000 taln2x-1.0.1/src/taln2x/utils/Event.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1695 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/utils/Track.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      111 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/utils/__init__.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     7990 2023-06-16 14:53:14.000000 taln2x-1.0.1/src/taln2x/utils/archives.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    14402 2023-06-20 15:36:12.000000 taln2x-1.0.1/src/taln2x/utils/easychair.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1888 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/utils/readevent.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     4324 2023-06-08 07:15:42.000000 taln2x-1.0.1/src/taln2x/utils/readpdf.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     7393 2023-06-23 08:03:17.000000 taln2x-1.0.1/src/taln2x/utils/sciencesconf.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     2570 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/utils/searchid.py
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     4585 2023-02-06 10:46:05.000000 taln2x-1.0.1/src/taln2x/utils/taln_archives_parser.py
-drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-23 14:00:31.908492 taln2x-1.0.1/src/taln2x.egg-info/
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     3107 2023-06-23 14:00:31.000000 taln2x-1.0.1/src/taln2x.egg-info/PKG-INFO
--rw-rw-r--   0 yparment  (1000) yparment  (1000)     1424 2023-06-23 14:00:31.000000 taln2x-1.0.1/src/taln2x.egg-info/SOURCES.txt
--rw-rw-r--   0 yparment  (1000) yparment  (1000)        1 2023-06-23 14:00:31.000000 taln2x-1.0.1/src/taln2x.egg-info/dependency_links.txt
--rw-rw-r--   0 yparment  (1000) yparment  (1000)       48 2023-06-23 14:00:31.000000 taln2x-1.0.1/src/taln2x.egg-info/entry_points.txt
--rw-rw-r--   0 yparment  (1000) yparment  (1000)      137 2023-06-23 14:00:31.000000 taln2x-1.0.1/src/taln2x.egg-info/requires.txt
--rw-rw-r--   0 yparment  (1000) yparment  (1000)        7 2023-06-23 14:00:31.000000 taln2x-1.0.1/src/taln2x.egg-info/top_level.txt
--rw-rw-r--   0 yparment  (1000) yparment  (1000)    11406 2023-02-06 10:46:05.000000 taln2x-1.0.1/taln2x.png
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.075765 taln2x-1.0.2/
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)       65 2023-02-16 14:40:42.000000 taln2x-1.0.2/.gitignore
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    35132 2023-02-06 10:46:05.000000 taln2x-1.0.2/LICENCE
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)       31 2023-06-23 13:55:10.000000 taln2x-1.0.2/MANIFEST.in
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     3259 2023-06-27 15:07:16.075765 taln2x-1.0.2/PKG-INFO
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     2540 2023-06-27 13:06:46.000000 taln2x-1.0.2/README.md
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1264 2023-06-08 07:15:42.000000 taln2x-1.0.2/pyproject.toml
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      137 2023-02-06 10:46:05.000000 taln2x-1.0.2/requirements.txt
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)       38 2023-06-27 15:07:16.075765 taln2x-1.0.2/setup.cfg
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.023764 taln2x-1.0.2/src/
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.023764 taln2x-1.0.2/src/taln2x/
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)       54 2023-06-27 15:05:30.000000 taln2x-1.0.2/src/taln2x/__init__.py
+-rwxrwxr-x   0 yparment  (1000) yparment  (1000)    20234 2023-06-15 07:48:27.000000 taln2x-1.0.2/src/taln2x/__main__.py
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.027764 taln2x-1.0.2/src/taln2x/exports/
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)       53 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/exports/__init__.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    15746 2023-06-15 11:55:11.000000 taln2x-1.0.2/src/taln2x/exports/anthology.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    14434 2023-06-20 07:52:12.000000 taln2x-1.0.2/src/taln2x/exports/archives.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     6215 2023-06-15 13:35:06.000000 taln2x-1.0.2/src/taln2x/exports/dblp.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    27712 2023-06-27 13:59:39.000000 taln2x-1.0.2/src/taln2x/exports/hal.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    15316 2023-06-23 15:20:56.000000 taln2x-1.0.2/src/taln2x/exports/pdf.py
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.071765 taln2x-1.0.2/src/taln2x/templates/
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)  3321771 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/PDFBox-0.7.3.jar
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    35605 2023-06-19 09:22:47.000000 taln2x-1.0.2/src/taln2x/templates/aofr.xsd
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      923 2023-02-16 15:02:01.000000 taln2x-1.0.2/src/taln2x/templates/articles.csv
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)  2280976 2023-02-16 15:07:58.000000 taln2x-1.0.2/src/taln2x/templates/articles.zip
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)  3223045 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/background.png
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      701 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/blank.pdf
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    59921 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/by.eps
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     2275 2023-02-17 16:26:28.000000 taln2x-1.0.2/src/taln2x/templates/config.toml
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1428 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/dblpsubmission.dtd
+-rwxrwxr-x   0 yparment  (1000) yparment  (1000)     9346 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/easy2acl.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      555 2023-02-16 15:05:52.000000 taln2x-1.0.2/src/taln2x/templates/event.yml
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     7921 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/logo.png
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     7657 2023-06-23 15:24:32.000000 taln2x-1.0.2/src/taln2x/templates/pre-proceedings-en.tex
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     7700 2023-06-23 15:25:49.000000 taln2x-1.0.2/src/taln2x/templates/pre-proceedings.tex
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     3704 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/templates/single_paper.tex
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     6408 2023-02-14 16:39:55.000000 taln2x-1.0.2/src/taln2x/templates/taln-archives.xsd
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.075765 taln2x-1.0.2/src/taln2x/utils/
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1014 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/utils/Article.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      591 2023-06-15 11:52:42.000000 taln2x-1.0.2/src/taln2x/utils/Author.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1469 2023-06-16 15:05:19.000000 taln2x-1.0.2/src/taln2x/utils/Event.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1695 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/utils/Track.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      111 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/utils/__init__.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     7990 2023-06-16 14:53:14.000000 taln2x-1.0.2/src/taln2x/utils/archives.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    14402 2023-06-20 15:36:12.000000 taln2x-1.0.2/src/taln2x/utils/easychair.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1888 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/utils/readevent.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     4324 2023-06-08 07:15:42.000000 taln2x-1.0.2/src/taln2x/utils/readpdf.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     7393 2023-06-23 08:03:17.000000 taln2x-1.0.2/src/taln2x/utils/sciencesconf.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     2570 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/utils/searchid.py
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     4585 2023-02-06 10:46:05.000000 taln2x-1.0.2/src/taln2x/utils/taln_archives_parser.py
+drwxrwxr-x   0 yparment  (1000) yparment  (1000)        0 2023-06-27 15:07:16.027764 taln2x-1.0.2/src/taln2x.egg-info/
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     3259 2023-06-27 15:07:16.000000 taln2x-1.0.2/src/taln2x.egg-info/PKG-INFO
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)     1424 2023-06-27 15:07:16.000000 taln2x-1.0.2/src/taln2x.egg-info/SOURCES.txt
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)        1 2023-06-27 15:07:16.000000 taln2x-1.0.2/src/taln2x.egg-info/dependency_links.txt
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)       48 2023-06-27 15:07:16.000000 taln2x-1.0.2/src/taln2x.egg-info/entry_points.txt
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)      137 2023-06-27 15:07:16.000000 taln2x-1.0.2/src/taln2x.egg-info/requires.txt
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)        7 2023-06-27 15:07:16.000000 taln2x-1.0.2/src/taln2x.egg-info/top_level.txt
+-rw-rw-r--   0 yparment  (1000) yparment  (1000)    11406 2023-02-06 10:46:05.000000 taln2x-1.0.2/taln2x.png
```

### Comparing `taln2x-1.0.1/LICENCE` & `taln2x-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/PKG-INFO` & `taln2x-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: taln2x
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command-line application to export (TALN-like) conference proceedings to various formats (namely pdf, hal, aclanthology, dblp)
 Author-email: Yannick Parmentier <yannick.parmentier@gmail.com>
 Project-URL: Homepage, https://gitlab.inria.fr/talnarchives/taln2x
 Project-URL: Bug Tracker, https://gitlab.inria.fr/talnarchives/taln2x/-/issues
 Keywords: taln,atala,paper,publication,open archive
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-![](taln2x.png)
+![](./taln2x.png)
 
 ## Description
-`taln2x` is a Python program which converts a set of scientific articles to a ready-to-ingest dataset for open archives. Currently supported output formats include pdf (for printable full proceedings), [TALNarchives](http://talnarchives.atala.org), [HAL](https://hal.science), [ACL anthology](https://aclanthology.org), and [DBLP](https://dblp.org).
+`taln2x` is a Python program which converts a set of scientific articles to a ready-to-ingest dataset for open archives. Currently supported output formats include pdf (for printable full proceedings), [TALN archives](http://talnarchives.atala.org), [HAL](https://hal.science), [ACL anthology](https://aclanthology.org), and [DBLP](https://dblp.org).
 
 ## User interface
-`taln2x` is a command-line tool which expects as input a directory containing specific pieces of information and relying on a given structure (see documentation) and outputs a ready-to-zip-and-upload directory whose internal structure depends on the target online archive.
+`taln2x` is a command-line tool which expects as input a directory containing specific pieces of information (gathered either manually or else via an abstract management system such as easychair) and relying on a given structure (see documentation), and outputs a directory whose internal structure depends on the target online archive.
 
-(asciinema animation to come)
+![](./mkdocs/docs/img/taln2x.gif)
 
 ## Installation
 The recommanded way to install `taln2x` is to use the `pip` package manager (within a virtual environment to avoid conflicts with installed libraries):
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install taln2x
 ```
 ## Basic usage
 
 ```bash
 taln2x COMMAND [OPTIONS]
 ```
-Where `COMMAND` is either `init` (to set up an input directory containing the expected structure and ready-to-fill config file) or `convert` (to read an input directory specified via the command line options or else via a configuration file named `.taln2x-config.toml`, see documentation).
+Where `COMMAND` is either `new` (to set up an input directory containing the expected structure and ready-to-fill config files), `build` (to compile proceedings in a given target format according to the config file, see documentation), `clean`  (to remove proceedings from output directory), or `list` (to check which articles can be found on the [HAL](https://hal.science) open archive).
 
 For a full list of options, invoke:
 ```bash
 taln2x --help
 ```
 
 ## Documentation
 
-`taln2x` documentation can be accessed via its webpage : [https://talnarchives.gitlabpages.inria.fr/taln2x](https://talnarchives.gitlabpages.inria.fr/taln2x).
+`taln2x` documentation is available at [https://talnarchives.gitlabpages.inria.fr/taln2x](https://talnarchives.gitlabpages.inria.fr/taln2x).
 
 ## Authors and acknowledgment
 `taln2x` has been developed by Yannick Parmentier, with the help of Sylvain Pogodalla, on behalf of [ATALA](https://atala.org) (the French Association for Computational Linguistics).
 
 The `taln2x` logo has been created using the [Letterblocks fonts](https://www.1001fonts.com/letterblocks-font.html) made by Vladimir Nikolic.
 
 ## License
```

### Comparing `taln2x-1.0.1/README.md` & `taln2x-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-![](taln2x.png)
+![](./taln2x.png)
 
 ## Description
-`taln2x` is a Python program which converts a set of scientific articles to a ready-to-ingest dataset for open archives. Currently supported output formats include pdf (for printable full proceedings), [TALNarchives](http://talnarchives.atala.org), [HAL](https://hal.science), [ACL anthology](https://aclanthology.org), and [DBLP](https://dblp.org).
+`taln2x` is a Python program which converts a set of scientific articles to a ready-to-ingest dataset for open archives. Currently supported output formats include pdf (for printable full proceedings), [TALN archives](http://talnarchives.atala.org), [HAL](https://hal.science), [ACL anthology](https://aclanthology.org), and [DBLP](https://dblp.org).
 
 ## User interface
-`taln2x` is a command-line tool which expects as input a directory containing specific pieces of information and relying on a given structure (see documentation) and outputs a ready-to-zip-and-upload directory whose internal structure depends on the target online archive.
+`taln2x` is a command-line tool which expects as input a directory containing specific pieces of information (gathered either manually or else via an abstract management system such as easychair) and relying on a given structure (see documentation), and outputs a directory whose internal structure depends on the target online archive.
 
-(asciinema animation to come)
+![](./mkdocs/docs/img/taln2x.gif)
 
 ## Installation
 The recommanded way to install `taln2x` is to use the `pip` package manager (within a virtual environment to avoid conflicts with installed libraries):
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install taln2x
 ```
 ## Basic usage
 
 ```bash
 taln2x COMMAND [OPTIONS]
 ```
-Where `COMMAND` is either `init` (to set up an input directory containing the expected structure and ready-to-fill config file) or `convert` (to read an input directory specified via the command line options or else via a configuration file named `.taln2x-config.toml`, see documentation).
+Where `COMMAND` is either `new` (to set up an input directory containing the expected structure and ready-to-fill config files), `build` (to compile proceedings in a given target format according to the config file, see documentation), `clean`  (to remove proceedings from output directory), or `list` (to check which articles can be found on the [HAL](https://hal.science) open archive).
 
 For a full list of options, invoke:
 ```bash
 taln2x --help
 ```
 
 ## Documentation
 
-`taln2x` documentation can be accessed via its webpage : [https://talnarchives.gitlabpages.inria.fr/taln2x](https://talnarchives.gitlabpages.inria.fr/taln2x).
+`taln2x` documentation is available at [https://talnarchives.gitlabpages.inria.fr/taln2x](https://talnarchives.gitlabpages.inria.fr/taln2x).
 
 ## Authors and acknowledgment
 `taln2x` has been developed by Yannick Parmentier, with the help of Sylvain Pogodalla, on behalf of [ATALA](https://atala.org) (the French Association for Computational Linguistics).
 
 The `taln2x` logo has been created using the [Letterblocks fonts](https://www.1001fonts.com/letterblocks-font.html) made by Vladimir Nikolic.
 
 ## License
```

### Comparing `taln2x-1.0.1/pyproject.toml` & `taln2x-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/__main__.py` & `taln2x-1.0.2/src/taln2x/__main__.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/exports/anthology.py` & `taln2x-1.0.2/src/taln2x/exports/anthology.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/exports/archives.py` & `taln2x-1.0.2/src/taln2x/exports/archives.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/exports/dblp.py` & `taln2x-1.0.2/src/taln2x/exports/dblp.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/exports/hal.py` & `taln2x-1.0.2/src/taln2x/exports/hal.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,16 @@
         else:
             ordered = order_papers(papers, order, stopwords, verbose, \
                                    event.__dict__['tracks'][t].__dict__['authors'])
         for art in tqdm.tqdm(ordered):
             if art:
                 write_hal_article(event, t, indir, os.path.join(outdir, eventname), \
                                   art, current_pos, bibfileh, behalfof, x_stamp_tag, \
-                                  include_pdf, guess, dry, update, no_meta, pdf_url, national)
+                                  include_pdf, guess, dry, update, no_meta, pdf_url, \
+                                  national, verbose)
                 current_pos += art.__dict__['numpages']
             else:
                 current_pos += 1 #skip session's delimiter
         ## Close file handler and write down BIB content (cf X2Hal)
         bibfileh.close()
         ## Prepare shell script for upload to HAL via cURL
         shellfile = os.path.join(outdir, eventname, \
@@ -138,15 +139,15 @@
                 f'\techo Processing article and file ${{i}} >> ../{logfile} ;\n'          
                 f'\tbash ${{i}} >> ../{logfile} ;',
                 f'\ndone\n']
         shellfileh.write(' '.join(curl))
         shellfileh.close()
 
 def write_hal_article(event, track, indir, outdir, art, current_pos, bibfileh, behalf, \
-                      stamptag, include_pdf, guess, dry, update, no_meta, base_url, national):
+                      stamptag, include_pdf, guess, dry, update, no_meta, base_url, national, verbose):
     paperid    = art.__dict__['paperid']
     xmlfile    = os.path.join(outdir, track, paperid + '.xml')
     #print('*', art)
     #print('**', list(map(lambda x: event.__dict__['tracks'][track].__dict__['authors'][paperid][x].__str__(), range(len(event.__dict__['tracks'][track].__dict__['authors'][paperid])))))
     # Preparing XML content (DOM)
     root       = ET.Element('TEI', xmlns="http://www.tei-c.org/ns/1.0")
     root.set("xmlns:hal","http://hal.archives-ouvertes.fr/")
@@ -163,25 +164,26 @@
     title.text = art.__dict__['title']
     title2     = ET.SubElement(tstmt, 'title')
     title2.set('xml:lang', html.unescape(art.__dict__['language2']))
     title2.text= art.__dict__['title2']
     affilia    = [] #name, country
     autbib     = [] #authors as bibtex strings
     try:
-        for au in event.__dict__['tracks'][track].__dict__['authors'][paperid]:
+        for au in event.__dict__['tracks'][track].__dict__['authors'][int(paperid)]:
             auteur  = ET.SubElement(tstmt, 'author', role="aut")
             autbib.append((re.sub(r'([^\\])~', r'\1 ', au.__dict__['firstname']), \
                            re.sub(r'([^\\])~', r'\1 ', au.__dict__['lastname'])))
             pers    = ET.SubElement(auteur, 'persName')
             ET.SubElement(pers, 'forename', type='first').text = au.__dict__['firstname'].replace('~', ' ')
             ET.SubElement(pers, 'surname').text                = au.__dict__['lastname'].replace('~', ' ')
             ET.SubElement(auteur,'affiliation',ref="#localStruct-"+str(au.__dict__['rank']))
             affilia.append(au.__dict__['affiliation'])
     except KeyError: #paperid not found in track's authors (cf author_list.xlsx)
-        print(f'[Warning] author unknown for paper {paperid}', file=sys.stderr)
+        if verbose > 0 :
+            print(f'[Warning] author unknown for paper {paperid}', file=sys.stderr)
         for aut2 in art.__dict__['authors'].replace(' and ', ', ').split(', '):
             aut     = re.sub(r'([^\\])~', r'\1 ', aut2) #replace unsplittable spaces
             auteur  = ET.SubElement(tstmt, 'author', role="aut")
             #fname  = aut.split(' ')[0]
             #lname  = ' '.join(aut.split(' ')[1:])
             fname   = HumanName(aut.strip()).first + ' ' + HumanName(aut.strip()).middle
             lname   = HumanName(aut.strip()).last
@@ -218,23 +220,24 @@
     bstruct = ET.SubElement(sdesc, 'biblStruct')
     analytic= ET.SubElement(bstruct, 'analytic')
     titleA  = ET.SubElement(analytic, 'title')
     titleA.set('xml:lang', art.__dict__['language'])
     titleA.text = art.__dict__['title']
     try:
         #print(paperid, sorted(event.__dict__['tracks'][track].__dict__['authors']))
-        for au in event.__dict__['tracks'][track].__dict__['authors'][paperid]:
+        for au in event.__dict__['tracks'][track].__dict__['authors'][int(paperid)]:
             auteurA  = ET.SubElement(analytic, 'author', role="aut")
             persA    = ET.SubElement(auteurA, 'persName')
             ET.SubElement(persA, 'forename', type='first').text = au.__dict__['firstname'].replace('~', ' ')
             ET.SubElement(persA, 'surname').text                = au.__dict__['lastname'].replace('~', ' ')
             ET.SubElement(auteurA, 'email').text = au.__dict__['email']
             ET.SubElement(auteurA, 'affiliation',ref="#localStruct-"+str(au.__dict__['rank']))
     except KeyError:
-        print(f'[Warning] author unknown for paper {paperid}', file=sys.stderr)
+        if verbose > 0:
+            print(f'[Warning] author unknown for paper {paperid}', file=sys.stderr)
         for aut2 in art.__dict__['authors'].replace(' and ', ', ').split(', '):
             aut      = re.sub(r'([^\\])~', r'\1 ', aut2)
             auteurA  = ET.SubElement(analytic, 'author', role="aut")
             #fname   = aut.split(' ')[0]
             #lname   = ' '.join(aut.split(' ')[1:])
             fname    = HumanName(aut.strip()).first + ' ' + HumanName(aut.strip()).middle
             lname    = HumanName(aut.strip()).last
```

### Comparing `taln2x-1.0.1/src/taln2x/exports/pdf.py` & `taln2x-1.0.2/src/taln2x/exports/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,17 @@
                                     event.__dict__['abbrev'])
         line_out = line_out.replace('SHORT-PLACEHOLDER',    \
                                     event.__dict__['shortbooktitle'])
         line_out = line_out.replace('YEAR-PLACEHOLDER',    \
                                     str(event.__dict__['year']))
         begin = event.__dict__['begin'].strftime('%Y-%m-%d')
         end   = event.__dict__['end'].strftime('%Y-%m-%d')
+        datestr = '{\\origdate \\daterange{' + begin + '}{' + end +'} }' if begin != end else '{\\origdate \\printdate{' + begin + '} }'
         line_out = line_out.replace('DATE-PLACEHOLDER',      \
-                                    '{\\origdate \\daterange{' + \
-                                    begin + '}{' + end +'} }')
+                                    datestr)
         line_out = line_out.replace('URL-PLACEHOLDER',      \
                                     str(event.__dict__['url']))
         line_out = line_out.replace('CHAIRS-PLACEHOLDER',     \
                                     chairs)
         line_out = line_out.replace('LOCATION-PLACEHOLDER',  \
                                     event.__dict__['location'])
         line_out = line_out.replace('PUBLISHER-PLACEHOLDER',  \
```

### Comparing `taln2x-1.0.1/src/taln2x/templates/PDFBox-0.7.3.jar` & `taln2x-1.0.2/src/taln2x/templates/PDFBox-0.7.3.jar`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/aofr.xsd` & `taln2x-1.0.2/src/taln2x/templates/aofr.xsd`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/articles.csv` & `taln2x-1.0.2/src/taln2x/templates/articles.csv`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/articles.zip` & `taln2x-1.0.2/src/taln2x/templates/articles.zip`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/background.png` & `taln2x-1.0.2/src/taln2x/templates/background.png`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/blank.pdf` & `taln2x-1.0.2/src/taln2x/templates/blank.pdf`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/by.eps` & `taln2x-1.0.2/src/taln2x/templates/by.eps`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/config.toml` & `taln2x-1.0.2/src/taln2x/templates/config.toml`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/dblpsubmission.dtd` & `taln2x-1.0.2/src/taln2x/templates/dblpsubmission.dtd`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/easy2acl.py` & `taln2x-1.0.2/src/taln2x/templates/easy2acl.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/event.yml` & `taln2x-1.0.2/src/taln2x/templates/event.yml`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/logo.png` & `taln2x-1.0.2/src/taln2x/templates/logo.png`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/pre-proceedings-en.tex` & `taln2x-1.0.2/src/taln2x/templates/pre-proceedings-en.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 %%%% SemDial Proceedings template by Raquel Fernández, 2013.
 %%%% Modified by Simon Dobnik for the proceedings of IWCS 2019.
 %%%% Modified by Yannick Parmentier and Sylvain Pogodalla for the proceedings of TALN 2020.
 
-\documentclass[a4paper,11pt,oneside]{book}
+\documentclass[a4paper,11pt,oneside,english]{book}
 
 \usepackage{times}
 \usepackage[a4paper,hmargin=1.2cm,top=1cm,bottom=2.5cm, includefoot=true, hcentering]{geometry}
 
 \setlength{\parindent}{0pt}
 
 \usepackage[english]{babel}
-\usepackage[english]{isodate}
+\usepackage[num]{isodate}
 \usepackage[utf8]{inputenc} 
 \usepackage[T1]{fontenc} % fonts to encode unicode
 \usepackage{changepage}  % for local redefinition of margins
+\selectlanguage{UKenglish}
 
 \usepackage{tabularx}
 \usepackage{tipa} 
 \usepackage{newunicodechar}
 \newunicodechar{ʁ}{\textipa{K}}
 \newunicodechar{ʒ}{\textipa{Z}}
 \newunicodechar{ʃ}{\textipa{S}}
```

### Comparing `taln2x-1.0.1/src/taln2x/templates/pre-proceedings.tex` & `taln2x-1.0.2/src/taln2x/templates/pre-proceedings.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 %%%% SemDial Proceedings template by Raquel Fernández, 2013.
 %%%% Modified by Simon Dobnik for the proceedings of IWCS 2019.
 %%%% Modified by Yannick Parmentier and Sylvain Pogodalla for the proceedings of TALN 2020.
 
-\documentclass[a4paper,11pt,oneside]{book}
+\documentclass[a4paper,11pt,oneside,french]{book}
 
 \usepackage{times}
 \usepackage[a4paper,hmargin=1.2cm,top=1cm,bottom=2.5cm, includefoot=true, hcentering]{geometry}
 
 \setlength{\parindent}{0pt}
 
 \usepackage[french]{babel}
-\usepackage[french]{isodate}
+\usepackage[num]{isodate}
 \usepackage[utf8]{inputenc} 
 \usepackage[T1]{fontenc} % fonts to encode unicode
 \usepackage{changepage}  % for local redefinition of margins
+\selectlanguage{french}
 
 \usepackage{tabularx}
 \usepackage{tipa} 
 \usepackage{newunicodechar}
 \newunicodechar{ʁ}{\textipa{K}}
 \newunicodechar{ʒ}{\textipa{Z}}
 \newunicodechar{ʃ}{\textipa{S}}
```

### Comparing `taln2x-1.0.1/src/taln2x/templates/single_paper.tex` & `taln2x-1.0.2/src/taln2x/templates/single_paper.tex`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/templates/taln-archives.xsd` & `taln2x-1.0.2/src/taln2x/templates/taln-archives.xsd`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/Article.py` & `taln2x-1.0.2/src/taln2x/utils/Article.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/Author.py` & `taln2x-1.0.2/src/taln2x/utils/Author.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/Event.py` & `taln2x-1.0.2/src/taln2x/utils/Event.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/Track.py` & `taln2x-1.0.2/src/taln2x/utils/Track.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/archives.py` & `taln2x-1.0.2/src/taln2x/utils/archives.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/easychair.py` & `taln2x-1.0.2/src/taln2x/utils/easychair.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/readevent.py` & `taln2x-1.0.2/src/taln2x/utils/readevent.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/readpdf.py` & `taln2x-1.0.2/src/taln2x/utils/readpdf.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/sciencesconf.py` & `taln2x-1.0.2/src/taln2x/utils/sciencesconf.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/searchid.py` & `taln2x-1.0.2/src/taln2x/utils/searchid.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x/utils/taln_archives_parser.py` & `taln2x-1.0.2/src/taln2x/utils/taln_archives_parser.py`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/src/taln2x.egg-info/PKG-INFO` & `taln2x-1.0.2/src/taln2x.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: taln2x
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command-line application to export (TALN-like) conference proceedings to various formats (namely pdf, hal, aclanthology, dblp)
 Author-email: Yannick Parmentier <yannick.parmentier@gmail.com>
 Project-URL: Homepage, https://gitlab.inria.fr/talnarchives/taln2x
 Project-URL: Bug Tracker, https://gitlab.inria.fr/talnarchives/taln2x/-/issues
 Keywords: taln,atala,paper,publication,open archive
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-![](taln2x.png)
+![](./taln2x.png)
 
 ## Description
-`taln2x` is a Python program which converts a set of scientific articles to a ready-to-ingest dataset for open archives. Currently supported output formats include pdf (for printable full proceedings), [TALNarchives](http://talnarchives.atala.org), [HAL](https://hal.science), [ACL anthology](https://aclanthology.org), and [DBLP](https://dblp.org).
+`taln2x` is a Python program which converts a set of scientific articles to a ready-to-ingest dataset for open archives. Currently supported output formats include pdf (for printable full proceedings), [TALN archives](http://talnarchives.atala.org), [HAL](https://hal.science), [ACL anthology](https://aclanthology.org), and [DBLP](https://dblp.org).
 
 ## User interface
-`taln2x` is a command-line tool which expects as input a directory containing specific pieces of information and relying on a given structure (see documentation) and outputs a ready-to-zip-and-upload directory whose internal structure depends on the target online archive.
+`taln2x` is a command-line tool which expects as input a directory containing specific pieces of information (gathered either manually or else via an abstract management system such as easychair) and relying on a given structure (see documentation), and outputs a directory whose internal structure depends on the target online archive.
 
-(asciinema animation to come)
+![](./mkdocs/docs/img/taln2x.gif)
 
 ## Installation
 The recommanded way to install `taln2x` is to use the `pip` package manager (within a virtual environment to avoid conflicts with installed libraries):
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install taln2x
 ```
 ## Basic usage
 
 ```bash
 taln2x COMMAND [OPTIONS]
 ```
-Where `COMMAND` is either `init` (to set up an input directory containing the expected structure and ready-to-fill config file) or `convert` (to read an input directory specified via the command line options or else via a configuration file named `.taln2x-config.toml`, see documentation).
+Where `COMMAND` is either `new` (to set up an input directory containing the expected structure and ready-to-fill config files), `build` (to compile proceedings in a given target format according to the config file, see documentation), `clean`  (to remove proceedings from output directory), or `list` (to check which articles can be found on the [HAL](https://hal.science) open archive).
 
 For a full list of options, invoke:
 ```bash
 taln2x --help
 ```
 
 ## Documentation
 
-`taln2x` documentation can be accessed via its webpage : [https://talnarchives.gitlabpages.inria.fr/taln2x](https://talnarchives.gitlabpages.inria.fr/taln2x).
+`taln2x` documentation is available at [https://talnarchives.gitlabpages.inria.fr/taln2x](https://talnarchives.gitlabpages.inria.fr/taln2x).
 
 ## Authors and acknowledgment
 `taln2x` has been developed by Yannick Parmentier, with the help of Sylvain Pogodalla, on behalf of [ATALA](https://atala.org) (the French Association for Computational Linguistics).
 
 The `taln2x` logo has been created using the [Letterblocks fonts](https://www.1001fonts.com/letterblocks-font.html) made by Vladimir Nikolic.
 
 ## License
```

### Comparing `taln2x-1.0.1/src/taln2x.egg-info/SOURCES.txt` & `taln2x-1.0.2/src/taln2x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taln2x-1.0.1/taln2x.png` & `taln2x-1.0.2/taln2x.png`

 * *Files identical despite different names*

