# Comparing `tmp/advertools-0.9.0.tar.gz` & `tmp/advertools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/advertools-0.9.0.tar", last modified: Sat Apr  4 03:34:10 2020, max compression
+gzip compressed data, was "dist/advertools-0.9.1.tar", last modified: Tue May 19 21:24:48 2020, max compression
```

## Comparing `advertools-0.9.0.tar` & `advertools-0.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/
--rw-r--r--   0 Elias      (501) staff       (20)     6061 2020-04-04 03:33:22.000000 advertools-0.9.0/HISTORY.rst
--rw-r--r--   0 Elias      (501) staff       (20)     1084 2020-03-18 00:38:34.000000 advertools-0.9.0/LICENSE
--rw-r--r--   0 Elias      (501) staff       (20)      242 2018-07-06 15:42:59.000000 advertools-0.9.0/MANIFEST.in
--rw-r--r--   0 Elias      (501) staff       (20)    18866 2020-04-04 03:34:10.000000 advertools-0.9.0/PKG-INFO
--rw-r--r--   0 Elias      (501) staff       (20)     8803 2020-04-04 03:16:49.000000 advertools-0.9.0/README.rst
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools/
--rw-r--r--   0 Elias      (501) staff       (20)      686 2020-04-03 23:36:21.000000 advertools-0.9.0/advertools/__init__.py
--rw-r--r--   0 Elias      (501) staff       (20)     3019 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/_yt_helpers.py
--rw-r--r--   0 Elias      (501) staff       (20)     3442 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/ad_create.py
--rw-r--r--   0 Elias      (501) staff       (20)     6561 2020-03-19 16:11:53.000000 advertools-0.9.0/advertools/ad_from_string.py
--rw-r--r--   0 Elias      (501) staff       (20)   878792 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/emoji.py
--rw-r--r--   0 Elias      (501) staff       (20)    31921 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/extract.py
--rw-r--r--   0 Elias      (501) staff       (20)    10866 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/kw_generate.py
--rw-r--r--   0 Elias      (501) staff       (20)     6650 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/regex.py
--rw-r--r--   0 Elias      (501) staff       (20)    57080 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/serp.py
--rw-r--r--   0 Elias      (501) staff       (20)    10566 2020-04-04 03:07:27.000000 advertools-0.9.0/advertools/sitemaps.py
--rw-r--r--   0 Elias      (501) staff       (20)   240761 2020-04-01 01:18:46.000000 advertools-0.9.0/advertools/stopwords.py
--rw-r--r--   0 Elias      (501) staff       (20)    55977 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/twitter.py
--rw-r--r--   0 Elias      (501) staff       (20)     1317 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/url_builders.py
--rw-r--r--   0 Elias      (501) staff       (20)    12285 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/word_frequency.py
--rw-r--r--   0 Elias      (501) staff       (20)     2752 2020-04-01 01:18:46.000000 advertools-0.9.0/advertools/word_tokenize.py
--rw-r--r--   0 Elias      (501) staff       (20)    70244 2020-03-18 00:32:17.000000 advertools-0.9.0/advertools/youtube.py
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/
--rw-r--r--   0 Elias      (501) staff       (20)    18866 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/PKG-INFO
--rw-r--r--   0 Elias      (501) staff       (20)     1675 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/SOURCES.txt
--rw-r--r--   0 Elias      (501) staff       (20)        1 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/dependency_links.txt
--rw-r--r--   0 Elias      (501) staff       (20)        1 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/not-zip-safe
--rw-r--r--   0 Elias      (501) staff       (20)       15 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/requires.txt
--rw-r--r--   0 Elias      (501) staff       (20)       11 2020-04-04 03:34:10.000000 advertools-0.9.0/advertools.egg-info/top_level.txt
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/docs/
--rw-r--r--   0 Elias      (501) staff       (20)      607 2018-07-06 16:35:47.000000 advertools-0.9.0/docs/Makefile
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/docs/_build/
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/docs/_build/html/
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/docs/_build/html/_static/
--rw-r--r--   0 Elias      (501) staff       (20)      286 2020-03-14 04:55:37.000000 advertools-0.9.0/docs/_build/html/_static/file.png
--rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-14 04:55:37.000000 advertools-0.9.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-14 04:55:37.000000 advertools-0.9.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 Elias      (501) staff       (20)       92 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.ad_create.rst
--rw-r--r--   0 Elias      (501) staff       (20)       97 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.ad_from_string.rst
--rw-r--r--   0 Elias      (501) staff       (20)      111 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.emoji.rst
--rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.extract.rst
--rw-r--r--   0 Elias      (501) staff       (20)       93 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.kw_generate.rst
--rw-r--r--   0 Elias      (501) staff       (20)       88 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.regex.rst
--rw-r--r--   0 Elias      (501) staff       (20)      526 2020-04-04 03:24:58.000000 advertools-0.9.0/docs/advertools.rst
--rw-r--r--   0 Elias      (501) staff       (20)       87 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.serp.rst
--rw-r--r--   0 Elias      (501) staff       (20)       90 2020-04-03 23:27:11.000000 advertools-0.9.0/docs/advertools.sitemaps.rst
--rw-r--r--   0 Elias      (501) staff       (20)       92 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.stopwords.rst
--rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.twitter.rst
--rw-r--r--   0 Elias      (501) staff       (20)       95 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.url_builders.rst
--rw-r--r--   0 Elias      (501) staff       (20)       97 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.word_frequency.rst
--rw-r--r--   0 Elias      (501) staff       (20)       96 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.word_tokenize.rst
--rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/advertools.youtube.rst
--rw-r--r--   0 Elias      (501) staff       (20)     5119 2020-03-20 04:32:55.000000 advertools-0.9.0/docs/conf.py
--rw-r--r--   0 Elias      (501) staff       (20)       54 2020-03-18 00:32:17.000000 advertools-0.9.0/docs/include_changelog.rst
--rw-r--r--   0 Elias      (501) staff       (20)     1550 2020-04-03 23:27:11.000000 advertools-0.9.0/docs/index.rst
--rw-r--r--   0 Elias      (501) staff       (20)      814 2018-07-06 16:35:47.000000 advertools-0.9.0/docs/make.bat
--rw-r--r--   0 Elias      (501) staff       (20)       67 2020-04-04 03:24:58.000000 advertools-0.9.0/docs/modules.rst
--rw-r--r--   0 Elias      (501) staff       (20)       27 2018-07-06 22:33:29.000000 advertools-0.9.0/docs/readme.rst
--rw-r--r--   0 Elias      (501) staff       (20)      452 2020-04-04 03:34:10.000000 advertools-0.9.0/setup.cfg
--rw-r--r--   0 Elias      (501) staff       (20)     1709 2020-04-03 23:36:21.000000 advertools-0.9.0/setup.py
-drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-04-04 03:34:10.000000 advertools-0.9.0/tests/
--rw-r--r--   0 Elias      (501) staff       (20)    20497 2018-07-06 15:39:13.000000 advertools-0.9.0/tests/.coverage
--rw-r--r--   0 Elias      (501) staff       (20)      419 2020-04-04 03:06:01.000000 advertools-0.9.0/tests/sitemap-index.xml
--rw-r--r--   0 Elias      (501) staff       (20)     1108 2020-04-03 23:27:11.000000 advertools-0.9.0/tests/sitemap.xml
--rw-r--r--   0 Elias      (501) staff       (20)      394 2020-04-03 23:27:11.000000 advertools-0.9.0/tests/sitemap.xml.gz
--rw-r--r--   0 Elias      (501) staff       (20)     1450 2018-07-11 14:25:26.000000 advertools-0.9.0/tests/test_ad_create.py
--rw-r--r--   0 Elias      (501) staff       (20)     1305 2020-03-18 00:30:00.000000 advertools-0.9.0/tests/test_ad_from_string.py
--rw-r--r--   0 Elias      (501) staff       (20)      522 2020-03-18 00:32:17.000000 advertools-0.9.0/tests/test_emoji.py
--rw-r--r--   0 Elias      (501) staff       (20)    14110 2020-03-18 00:32:17.000000 advertools-0.9.0/tests/test_extract.py
--rw-r--r--   0 Elias      (501) staff       (20)     6724 2020-03-18 00:30:00.000000 advertools-0.9.0/tests/test_kw_generate.py
--rw-r--r--   0 Elias      (501) staff       (20)     4945 2020-03-18 00:32:17.000000 advertools-0.9.0/tests/test_serp.py
--rw-r--r--   0 Elias      (501) staff       (20)      774 2020-04-04 03:12:41.000000 advertools-0.9.0/tests/test_sitemaps.py
--rw-r--r--   0 Elias      (501) staff       (20)     8523 2020-03-18 00:30:00.000000 advertools-0.9.0/tests/test_twitter.py
--rw-r--r--   0 Elias      (501) staff       (20)     1055 2018-07-11 15:04:09.000000 advertools-0.9.0/tests/test_url_builders.py
--rw-r--r--   0 Elias      (501) staff       (20)     1537 2020-03-18 00:30:00.000000 advertools-0.9.0/tests/test_word_frequency.py
--rw-r--r--   0 Elias      (501) staff       (20)      443 2020-03-18 00:32:17.000000 advertools-0.9.0/tests/test_word_tokenize.py
--rw-r--r--   0 Elias      (501) staff       (20)     6646 2020-03-18 00:32:17.000000 advertools-0.9.0/tests/test_youtube.py
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/
+-rw-r--r--   0 Elias      (501) staff       (20)     6615 2020-05-19 20:56:57.000000 advertools-0.9.1/HISTORY.rst
+-rw-r--r--   0 Elias      (501) staff       (20)     1084 2020-03-18 00:38:34.000000 advertools-0.9.1/LICENSE
+-rw-r--r--   0 Elias      (501) staff       (20)      242 2018-07-06 15:42:59.000000 advertools-0.9.1/MANIFEST.in
+-rw-r--r--   0 Elias      (501) staff       (20)    19540 2020-05-19 21:24:48.000000 advertools-0.9.1/PKG-INFO
+-rw-r--r--   0 Elias      (501) staff       (20)     8803 2020-05-19 20:32:37.000000 advertools-0.9.1/README.rst
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools/
+-rw-r--r--   0 Elias      (501) staff       (20)      686 2020-05-19 21:13:26.000000 advertools-0.9.1/advertools/__init__.py
+-rw-r--r--   0 Elias      (501) staff       (20)     3019 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/_yt_helpers.py
+-rw-r--r--   0 Elias      (501) staff       (20)     3442 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/ad_create.py
+-rw-r--r--   0 Elias      (501) staff       (20)     6561 2020-03-19 16:11:53.000000 advertools-0.9.1/advertools/ad_from_string.py
+-rw-r--r--   0 Elias      (501) staff       (20)   878792 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/emoji.py
+-rw-r--r--   0 Elias      (501) staff       (20)    31921 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/extract.py
+-rw-r--r--   0 Elias      (501) staff       (20)    10866 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/kw_generate.py
+-rw-r--r--   0 Elias      (501) staff       (20)     6650 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/regex.py
+-rw-r--r--   0 Elias      (501) staff       (20)    57080 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/serp.py
+-rw-r--r--   0 Elias      (501) staff       (20)    21827 2020-05-19 20:36:10.000000 advertools-0.9.1/advertools/sitemaps.py
+-rw-r--r--   0 Elias      (501) staff       (20)   241323 2020-05-19 20:32:46.000000 advertools-0.9.1/advertools/stopwords.py
+-rw-r--r--   0 Elias      (501) staff       (20)    55977 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/twitter.py
+-rw-r--r--   0 Elias      (501) staff       (20)     1317 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/url_builders.py
+-rw-r--r--   0 Elias      (501) staff       (20)    12285 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/word_frequency.py
+-rw-r--r--   0 Elias      (501) staff       (20)     2752 2020-05-13 14:05:51.000000 advertools-0.9.1/advertools/word_tokenize.py
+-rw-r--r--   0 Elias      (501) staff       (20)    70244 2020-03-18 00:32:17.000000 advertools-0.9.1/advertools/youtube.py
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/
+-rw-r--r--   0 Elias      (501) staff       (20)    19540 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/PKG-INFO
+-rw-r--r--   0 Elias      (501) staff       (20)     1675 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/SOURCES.txt
+-rw-r--r--   0 Elias      (501) staff       (20)        1 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/dependency_links.txt
+-rw-r--r--   0 Elias      (501) staff       (20)        1 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/not-zip-safe
+-rw-r--r--   0 Elias      (501) staff       (20)       15 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/requires.txt
+-rw-r--r--   0 Elias      (501) staff       (20)       11 2020-05-19 21:24:48.000000 advertools-0.9.1/advertools.egg-info/top_level.txt
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/docs/
+-rw-r--r--   0 Elias      (501) staff       (20)      607 2018-07-06 16:35:47.000000 advertools-0.9.1/docs/Makefile
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/docs/_build/
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/docs/_build/html/
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/docs/_build/html/_static/
+-rw-r--r--   0 Elias      (501) staff       (20)      286 2020-03-14 04:55:37.000000 advertools-0.9.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-14 04:55:37.000000 advertools-0.9.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 Elias      (501) staff       (20)       90 2020-03-14 04:55:37.000000 advertools-0.9.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 Elias      (501) staff       (20)      274 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.ad_create.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      255 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.ad_from_string.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      268 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.emoji.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      350 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.extract.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      308 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.kw_generate.rst
+-rw-r--r--   0 Elias      (501) staff       (20)       88 2020-03-18 00:32:17.000000 advertools-0.9.1/docs/advertools.regex.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      526 2020-05-19 21:12:10.000000 advertools-0.9.1/docs/advertools.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      293 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.serp.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      302 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.sitemaps.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      226 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.stopwords.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      272 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.twitter.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      220 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.url_builders.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      357 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.word_frequency.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      258 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.word_tokenize.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      270 2020-05-19 20:32:38.000000 advertools-0.9.1/docs/advertools.youtube.rst
+-rw-r--r--   0 Elias      (501) staff       (20)     5119 2020-03-20 04:32:55.000000 advertools-0.9.1/docs/conf.py
+-rw-r--r--   0 Elias      (501) staff       (20)       54 2020-03-18 00:32:17.000000 advertools-0.9.1/docs/include_changelog.rst
+-rw-r--r--   0 Elias      (501) staff       (20)     1716 2020-05-19 20:41:40.000000 advertools-0.9.1/docs/index.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      814 2018-07-06 16:35:47.000000 advertools-0.9.1/docs/make.bat
+-rw-r--r--   0 Elias      (501) staff       (20)       67 2020-05-19 21:12:10.000000 advertools-0.9.1/docs/modules.rst
+-rw-r--r--   0 Elias      (501) staff       (20)       27 2018-07-06 22:33:29.000000 advertools-0.9.1/docs/readme.rst
+-rw-r--r--   0 Elias      (501) staff       (20)      452 2020-05-19 21:24:48.000000 advertools-0.9.1/setup.cfg
+-rw-r--r--   0 Elias      (501) staff       (20)     1709 2020-05-19 21:13:26.000000 advertools-0.9.1/setup.py
+drwxr-xr-x   0 Elias      (501) staff       (20)        0 2020-05-19 21:24:48.000000 advertools-0.9.1/tests/
+-rw-r--r--   0 Elias      (501) staff       (20)    20497 2018-07-06 15:39:13.000000 advertools-0.9.1/tests/.coverage
+-rw-r--r--   0 Elias      (501) staff       (20)      419 2020-05-19 20:32:38.000000 advertools-0.9.1/tests/sitemap-index.xml
+-rw-r--r--   0 Elias      (501) staff       (20)     1108 2020-05-13 14:05:51.000000 advertools-0.9.1/tests/sitemap.xml
+-rw-r--r--   0 Elias      (501) staff       (20)      394 2020-05-13 14:05:51.000000 advertools-0.9.1/tests/sitemap.xml.gz
+-rw-r--r--   0 Elias      (501) staff       (20)     1450 2018-07-11 14:25:26.000000 advertools-0.9.1/tests/test_ad_create.py
+-rw-r--r--   0 Elias      (501) staff       (20)     1305 2020-03-18 00:30:00.000000 advertools-0.9.1/tests/test_ad_from_string.py
+-rw-r--r--   0 Elias      (501) staff       (20)      522 2020-03-18 00:32:17.000000 advertools-0.9.1/tests/test_emoji.py
+-rw-r--r--   0 Elias      (501) staff       (20)    14110 2020-03-18 00:32:17.000000 advertools-0.9.1/tests/test_extract.py
+-rw-r--r--   0 Elias      (501) staff       (20)     6724 2020-03-18 00:30:00.000000 advertools-0.9.1/tests/test_kw_generate.py
+-rw-r--r--   0 Elias      (501) staff       (20)     4945 2020-03-18 00:32:17.000000 advertools-0.9.1/tests/test_serp.py
+-rw-r--r--   0 Elias      (501) staff       (20)      774 2020-05-19 20:32:38.000000 advertools-0.9.1/tests/test_sitemaps.py
+-rw-r--r--   0 Elias      (501) staff       (20)     8523 2020-03-18 00:30:00.000000 advertools-0.9.1/tests/test_twitter.py
+-rw-r--r--   0 Elias      (501) staff       (20)     1055 2018-07-11 15:04:09.000000 advertools-0.9.1/tests/test_url_builders.py
+-rw-r--r--   0 Elias      (501) staff       (20)     1537 2020-03-18 00:30:00.000000 advertools-0.9.1/tests/test_word_frequency.py
+-rw-r--r--   0 Elias      (501) staff       (20)      443 2020-03-18 00:32:17.000000 advertools-0.9.1/tests/test_word_tokenize.py
+-rw-r--r--   0 Elias      (501) staff       (20)     6646 2020-03-18 00:32:17.000000 advertools-0.9.1/tests/test_youtube.py
```

### Comparing `advertools-0.9.0/HISTORY.rst` & `advertools-0.9.1/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 =======================
 Change Log - advertools
 =======================
 
+0.9.1 (2020-05-19)
+------------------
+
+* Added
+    - Ability to specify robots.txt file for ``sitemap_to_df``
+    - Ability to retreive any kind of sitemap (news, video, or images)
+    - Errors column to the returnd DataFrame if any errors occur
+    - A new ``sitemap_downloaded`` column showing datetime of getting the
+      sitemap
+
+* Fixed
+    - Logging issue causing ``sitemap_to_df`` to log the same action twice
+    - Issue preventing URLs not ending with xml or gz from being retreived
+    - Correct sitemap URL showing in the ``sitemap`` column
+
 0.9.0 (2020-04-03)
 ------------------
 
 * Added
     - New function ``sitemap_to_df`` imports an XML sitemap into a
       ``DataFrame``
```

### Comparing `advertools-0.9.0/LICENSE` & `advertools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/PKG-INFO` & `advertools-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: advertools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Productivity and analysis tools for online marketing
 Home-page: https://github.com/eliasdabbas/advertools
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: MIT license
 Description: .. image:: https://img.shields.io/pypi/v/advertools.svg
                 :target: https://pypi.python.org/pypi/advertools
@@ -195,14 +195,29 @@
         .. _extract entities from social media posts: http://bit.ly/2wTWvBI
         
         
         =======================
         Change Log - advertools
         =======================
         
+        0.9.1 (2020-05-19)
+        ------------------
+        
+        * Added
+            - Ability to specify robots.txt file for ``sitemap_to_df``
+            - Ability to retreive any kind of sitemap (news, video, or images)
+            - Errors column to the returnd DataFrame if any errors occur
+            - A new ``sitemap_downloaded`` column showing datetime of getting the
+              sitemap
+        
+        * Fixed
+            - Logging issue causing ``sitemap_to_df`` to log the same action twice
+            - Issue preventing URLs not ending with xml or gz from being retreived
+            - Correct sitemap URL showing in the ``sitemap`` column
+        
         0.9.0 (2020-04-03)
         ------------------
         
         * Added
             - New function ``sitemap_to_df`` imports an XML sitemap into a
               ``DataFrame``
```

### Comparing `advertools-0.9.0/README.rst` & `advertools-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/__init__.py` & `advertools-0.9.1/advertools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 """Top-level package for advertools."""
 
 __author__ = """Elias Dabbas"""
 __email__ = 'eliasdabbas@gmail.com'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 from advertools.ad_create import ad_create
 from advertools.ad_from_string import ad_from_string
 from advertools.emoji import emoji_search, emoji_df
 from advertools.extract import *
 from advertools.kw_generate import *
 from advertools.regex import *
```

### Comparing `advertools-0.9.0/advertools/_yt_helpers.py` & `advertools-0.9.1/advertools/_yt_helpers.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/ad_create.py` & `advertools-0.9.1/advertools/ad_create.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/ad_from_string.py` & `advertools-0.9.1/advertools/ad_from_string.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/emoji.py` & `advertools-0.9.1/advertools/emoji.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/extract.py` & `advertools-0.9.1/advertools/extract.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/kw_generate.py` & `advertools-0.9.1/advertools/kw_generate.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/regex.py` & `advertools-0.9.1/advertools/regex.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/serp.py` & `advertools-0.9.1/advertools/serp.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/stopwords.py` & `advertools-0.9.1/advertools/stopwords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,86 @@
 """
 .. _stopwords:
 
 Stopwords in Several Languages
 ==============================
 
+List of stopwords by the spaCy [#spaCy]_ package, useful in text mining,
+analyzing content of social media posts, tweets, web pages, keywords, etc.
 
-Stopwords by the spaCy package
-Copyright (C) 2016 ExplosionAI UG (haftungsbeschränkt), 2016 spaCy GmbH,
-2015 Matthew Honnibal
-
-List of stopwords useful in text mining, analyzing content of tweets, web
-pages, keywords, etc.
-
-Each list is accessible as part of a dictionary `stopwords` which is a normal
+Each list is accessible as part of a dictionary ``stopwords`` which is a normal
 Python dictionary.
 
+Available Languages:
+^^^^^^^^^^^^^^^^^^^^
+
+* Arabic
+* Azerbaijani
+* Bengali
+* Catalan
+* Chinese
+* Croatian
+* Danish
+* Dutch
+* English
+* Finnish
+* French
+* German
+* Greek
+* Hebrew
+* Hindi
+* Hungarian
+* Indonesian
+* Irish
+* Italian
+* Japanese
+* Kazakh
+* Nepali
+* Norwegian
+* Persian
+* Polish
+* Portuguese
+* Romanian
+* Russian
+* Sinhala
+* Spanish
+* Swedish
+* Tagalog
+* Tamil
+* Tatar
+* Telugu
+* Thai
+* Turkish
+* Ukrainian
+* Urdu
+* Vietnamese
 
 >>> import advertools as adv
->>> adv.stopwords['english'][:5]
+>>> sorted(adv.stopwords['english'])[:5]
 ["a", "about", "above", "across", "after"]
 
->>> adv.stopwords['german'][:5]
+>>> sorted(adv.stopwords['german'])[:5]
 ["a", "ab", "aber", "ach", "acht"]
 
+To get a list of all available languages, run
+
 >>> adv.stopwords.keys()
 dict_keys(['arabic', 'azerbaijani', 'bengali', 'catalan', 'chinese',
 'croatian', 'danish', 'dutch', 'english', 'finnish', 'french',
 'german', 'greek', 'hebrew', 'hindi', 'hungarian', 'indonesian',
 'irish', 'italian', 'japanese', 'kazakh', 'nepali', 'norwegian',
 'persian', 'polish', 'portuguese', 'romanian', 'russian', 'sinhala',
 'spanish', 'swedish', 'tagalog', 'tamil', 'tatar', 'telugu', 'thai',
 'turkish', 'ukrainian', 'urdu', 'vietnamese'])
+
+.. rubric:: Footnotes
+
+.. [#spaCy] Copyright (C) 2016 ExplosionAI UG (haftungsbeschränkt), 2016 spaCy GmbH,
+   2015 Matthew Honnibal
+
 """
 
 stopwords = dict(
 
 
 arabic={
     "آل", "آه", "آها", "آي", "أبو", "أثناء", "أحد", "أصبح", "أضحى", "أف",
```

### Comparing `advertools-0.9.0/advertools/twitter.py` & `advertools-0.9.1/advertools/twitter.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/url_builders.py` & `advertools-0.9.1/advertools/url_builders.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/word_frequency.py` & `advertools-0.9.1/advertools/word_frequency.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/word_tokenize.py` & `advertools-0.9.1/advertools/word_tokenize.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools/youtube.py` & `advertools-0.9.1/advertools/youtube.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/advertools.egg-info/PKG-INFO` & `advertools-0.9.1/advertools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: advertools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Productivity and analysis tools for online marketing
 Home-page: https://github.com/eliasdabbas/advertools
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: MIT license
 Description: .. image:: https://img.shields.io/pypi/v/advertools.svg
                 :target: https://pypi.python.org/pypi/advertools
@@ -195,14 +195,29 @@
         .. _extract entities from social media posts: http://bit.ly/2wTWvBI
         
         
         =======================
         Change Log - advertools
         =======================
         
+        0.9.1 (2020-05-19)
+        ------------------
+        
+        * Added
+            - Ability to specify robots.txt file for ``sitemap_to_df``
+            - Ability to retreive any kind of sitemap (news, video, or images)
+            - Errors column to the returnd DataFrame if any errors occur
+            - A new ``sitemap_downloaded`` column showing datetime of getting the
+              sitemap
+        
+        * Fixed
+            - Logging issue causing ``sitemap_to_df`` to log the same action twice
+            - Issue preventing URLs not ending with xml or gz from being retreived
+            - Correct sitemap URL showing in the ``sitemap`` column
+        
         0.9.0 (2020-04-03)
         ------------------
         
         * Added
             - New function ``sitemap_to_df`` imports an XML sitemap into a
               ``DataFrame``
```

### Comparing `advertools-0.9.0/advertools.egg-info/SOURCES.txt` & `advertools-0.9.1/advertools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/docs/Makefile` & `advertools-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/docs/advertools.rst` & `advertools-0.9.1/docs/advertools.rst`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/docs/conf.py` & `advertools-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/docs/index.rst` & `advertools-0.9.1/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,19 @@
    sphinx-quickstart on Fri Jul  6 20:35:47 2018.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 .. meta::
    :google-site-verification: GcN6XL_hWV3BP2Y9FNLjmTXxysS7QxJs804KoF15n_c
 
+.. meta::
+    :description lang=en:
+        Get productive as an online marketer with a Python package that helps
+        in automating many of the important tasks.
+
 advertools
 ==========
 Online marketing productivity and analysis tools
 ------------------------------------------------
 
 Generate keywords for SEM campaigns, create text ads on a large scale, analyze
 multiple SERPs at once, gain insights from large social media posts, and get
@@ -21,15 +26,15 @@
 .. toctree::
    :maxdepth: 2
    :titlesonly:
 
    About advertools <readme>
    Generate SEM Keywords <advertools.kw_generate>
    Create Text Ads on a Large Scale <advertools.ad_create>
-   Cretae Text Ads From Description Text <advertools.ad_from_string>
+   Create Text Ads From Description Text <advertools.ad_from_string>
    Emoji Tools <advertools.emoji>
    Extract Structured Entities from Text <advertools.extract>
    XML Sitemaps <advertools.sitemaps>
    Stop Words <advertools.stopwords>
    Text Analysis (absolute & weighted word frequency) <advertools.word_frequency>
    Word Tokenization (N-grams) <advertools.word_tokenize>
    Analyze Search Engine Results (SERPs) <advertools.serp>
```

### Comparing `advertools-0.9.0/docs/make.bat` & `advertools-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/setup.py` & `advertools-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
              'seo sem bingads keyword-research',
     name='advertools',
     packages=find_packages(include=['advertools']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eliasdabbas/advertools',
-    version='0.9.0',
+    version='0.9.1',
     zip_safe=False,
 )
```

### Comparing `advertools-0.9.0/tests/.coverage` & `advertools-0.9.1/tests/.coverage`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/sitemap.xml` & `advertools-0.9.1/tests/sitemap.xml`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_ad_create.py` & `advertools-0.9.1/tests/test_ad_create.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_ad_from_string.py` & `advertools-0.9.1/tests/test_ad_from_string.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_emoji.py` & `advertools-0.9.1/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_extract.py` & `advertools-0.9.1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_kw_generate.py` & `advertools-0.9.1/tests/test_kw_generate.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_serp.py` & `advertools-0.9.1/tests/test_serp.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_sitemaps.py` & `advertools-0.9.1/tests/test_sitemaps.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_twitter.py` & `advertools-0.9.1/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_url_builders.py` & `advertools-0.9.1/tests/test_url_builders.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_word_frequency.py` & `advertools-0.9.1/tests/test_word_frequency.py`

 * *Files identical despite different names*

### Comparing `advertools-0.9.0/tests/test_youtube.py` & `advertools-0.9.1/tests/test_youtube.py`

 * *Files identical despite different names*

