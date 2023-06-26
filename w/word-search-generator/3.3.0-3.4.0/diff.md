# Comparing `tmp/word-search-generator-3.3.0.tar.gz` & `tmp/word-search-generator-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "word-search-generator-3.3.0.tar", last modified: Tue May  2 16:12:33 2023, max compression
+gzip compressed data, was "word-search-generator-3.4.0.tar", last modified: Mon Jun 26 22:02:28 2023, max compression
```

## Comparing `word-search-generator-3.3.0.tar` & `word-search-generator-3.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.793887 word-search-generator-3.3.0/
--rw-r--r--   0 jbd        (501) staff       (20)       51 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/.flake8
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.695141 word-search-generator-3.3.0/.github/
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.732013 word-search-generator-3.3.0/.github/workflows/
--rw-r--r--   0 jbd        (501) staff       (20)      623 2022-10-24 19:07:34.000000 word-search-generator-3.3.0/.github/workflows/tests.yml
--rw-r--r--   0 jbd        (501) staff       (20)     1978 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/.gitignore
--rw-r--r--   0 jbd        (501) staff       (20)      961 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jbd        (501) staff       (20)    14802 2023-05-02 15:59:25.000000 word-search-generator-3.3.0/CHANGLOG.md
--rw-r--r--   0 jbd        (501) staff       (20)     1077 2022-12-02 16:21:47.000000 word-search-generator-3.3.0/LICENSE
--rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-05-02 16:12:33.792548 word-search-generator-3.3.0/PKG-INFO
--rw-r--r--   0 jbd        (501) staff       (20)     6954 2023-03-16 21:31:14.000000 word-search-generator-3.3.0/README.md
--rw-r--r--   0 jbd        (501) staff       (20)      383 2023-03-16 21:34:27.000000 word-search-generator-3.3.0/TODO.md
--rw-r--r--   0 jbd        (501) staff       (20)     2650 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/pyproject.toml
--rw-r--r--   0 jbd        (501) staff       (20)      157 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/requirements-dev.txt
--rw-r--r--   0 jbd        (501) staff       (20)       38 2023-01-20 23:10:24.000000 word-search-generator-3.3.0/requirements.txt
--rwxr-xr-x   0 jbd        (501) staff       (20)     1384 2023-03-06 05:27:14.000000 word-search-generator-3.3.0/run
--rw-r--r--   0 jbd        (501) staff       (20)       38 2023-05-02 16:12:33.794777 word-search-generator-3.3.0/setup.cfg
--rw-r--r--   0 jbd        (501) staff       (20)       38 2022-10-24 15:15:00.000000 word-search-generator-3.3.0/setup.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.696725 word-search-generator-3.3.0/src/
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.741589 word-search-generator-3.3.0/src/word_search_generator/
--rw-r--r--   0 jbd        (501) staff       (20)    22173 2023-05-02 15:59:25.000000 word-search-generator-3.3.0/src/word_search_generator/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)      119 2022-12-02 04:41:56.000000 word-search-generator-3.3.0/src/word_search_generator/__main__.py
--rw-r--r--   0 jbd        (501) staff       (20)     7856 2023-03-16 18:18:19.000000 word-search-generator-3.3.0/src/word_search_generator/cli.py
--rw-r--r--   0 jbd        (501) staff       (20)     1174 2023-01-09 17:44:57.000000 word-search-generator-3.3.0/src/word_search_generator/config.py
--rw-r--r--   0 jbd        (501) staff       (20)     6360 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/src/word_search_generator/export.py
--rw-r--r--   0 jbd        (501) staff       (20)     7847 2023-01-10 03:52:45.000000 word-search-generator-3.3.0/src/word_search_generator/generate.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.757199 word-search-generator-3.3.0/src/word_search_generator/mask/
--rw-r--r--   0 jbd        (501) staff       (20)    11610 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)     4202 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/bitmap.py
--rw-r--r--   0 jbd        (501) staff       (20)     3694 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/ellipse.py
--rw-r--r--   0 jbd        (501) staff       (20)    14385 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/polygon.py
--rw-r--r--   0 jbd        (501) staff       (20)    13001 2023-05-02 15:59:25.000000 word-search-generator-3.3.0/src/word_search_generator/mask/shapes.py
--rw-r--r--   0 jbd        (501) staff       (20)        0 2021-09-14 03:56:24.000000 word-search-generator-3.3.0/src/word_search_generator/py.typed
--rw-r--r--   0 jbd        (501) staff       (20)    23777 2023-05-02 15:59:36.000000 word-search-generator-3.3.0/src/word_search_generator/utils.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.759165 word-search-generator-3.3.0/src/word_search_generator/word/
--rw-r--r--   0 jbd        (501) staff       (20)     6873 2023-01-10 03:52:45.000000 word-search-generator-3.3.0/src/word_search_generator/word/__init__.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.752241 word-search-generator-3.3.0/src/word_search_generator.egg-info/
--rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/PKG-INFO
--rw-r--r--   0 jbd        (501) staff       (20)     1450 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/SOURCES.txt
--rw-r--r--   0 jbd        (501) staff       (20)        1 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/dependency_links.txt
--rw-r--r--   0 jbd        (501) staff       (20)       63 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/entry_points.txt
--rw-r--r--   0 jbd        (501) staff       (20)      180 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/requires.txt
--rw-r--r--   0 jbd        (501) staff       (20)       22 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/top_level.txt
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.767467 word-search-generator-3.3.0/tests/
--rw-r--r--   0 jbd        (501) staff       (20)    14859 2023-03-16 18:31:53.000000 word-search-generator-3.3.0/tests/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)    15204 2023-03-16 18:23:55.000000 word-search-generator-3.3.0/tests/test_Mask.py
--rw-r--r--   0 jbd        (501) staff       (20)     1188 2022-12-02 04:41:56.000000 word-search-generator-3.3.0/tests/test_Word.py
--rw-r--r--   0 jbd        (501) staff       (20)    12465 2023-03-16 21:43:26.000000 word-search-generator-3.3.0/tests/test_WordSearch.py
--rw-r--r--   0 jbd        (501) staff       (20)     5761 2023-03-16 18:25:31.000000 word-search-generator-3.3.0/tests/test_cli.py
--rw-r--r--   0 jbd        (501) staff       (20)     8797 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/tests/test_export.py
--rw-r--r--   0 jbd        (501) staff       (20)     2556 2023-01-10 03:52:45.000000 word-search-generator-3.3.0/tests/test_generate.py
--rw-r--r--   0 jbd        (501) staff       (20)     1317 2023-03-16 18:22:16.000000 word-search-generator-3.3.0/tests/test_shapes.py
--rw-r--r--   0 jbd        (501) staff       (20)     2392 2023-03-15 21:02:57.000000 word-search-generator-3.3.0/tests/test_utils.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.778143 word-search-generator-3.3.0/tools/
--rw-r--r--   0 jbd        (501) staff       (20)      385 2023-03-16 18:09:20.000000 word-search-generator-3.3.0/tools/build_masks_output_dict.py
--rw-r--r--   0 jbd        (501) staff       (20)     1125 2023-01-03 03:25:46.000000 word-search-generator-3.3.0/tools/pdf_layout_testing.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.789590 word-search-generator-3.3.0/tools/sample_word_lists/
--rw-r--r--   0 jbd        (501) staff       (20)       76 2021-08-19 05:15:03.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-10.txt
--rw-r--r--   0 jbd        (501) staff       (20)      173 2021-08-19 05:15:05.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-25.txt
--rw-r--r--   0 jbd        (501) staff       (20)       43 2021-08-19 05:15:01.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-5.txt
--rw-r--r--   0 jbd        (501) staff       (20)      369 2021-08-19 05:15:06.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-50.txt
--rw-r--r--   0 jbd        (501) staff       (20)       83 2021-08-19 05:15:08.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-junk.txt
--rw-r--r--   0 jbd        (501) staff       (20)      523 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/tox.ini
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.193896 word-search-generator-3.4.0/
+-rw-r--r--   0 jbd        (501) staff       (20)       51 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/.flake8
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.178699 word-search-generator-3.4.0/.github/
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.183230 word-search-generator-3.4.0/.github/workflows/
+-rw-r--r--   0 jbd        (501) staff       (20)      623 2022-10-24 16:01:30.000000 word-search-generator-3.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 jbd        (501) staff       (20)     1978 2023-03-13 16:13:15.000000 word-search-generator-3.4.0/.gitignore
+-rw-r--r--   0 jbd        (501) staff       (20)      961 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 jbd        (501) staff       (20)    15126 2023-06-26 21:43:27.000000 word-search-generator-3.4.0/CHANGLOG.md
+-rw-r--r--   0 jbd        (501) staff       (20)     1077 2021-08-08 03:10:36.000000 word-search-generator-3.4.0/LICENSE
+-rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-06-26 22:02:28.193714 word-search-generator-3.4.0/PKG-INFO
+-rw-r--r--   0 jbd        (501) staff       (20)     6954 2023-03-16 21:28:47.000000 word-search-generator-3.4.0/README.md
+-rw-r--r--   0 jbd        (501) staff       (20)      514 2023-06-03 05:23:36.000000 word-search-generator-3.4.0/TODO.md
+-rw-r--r--   0 jbd        (501) staff       (20)     2650 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/pyproject.toml
+-rw-r--r--   0 jbd        (501) staff       (20)      157 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/requirements-dev.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/requirements.txt
+-rwxr--r--   0 jbd        (501) staff       (20)     1384 2023-05-11 17:36:26.000000 word-search-generator-3.4.0/run
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2023-06-26 22:02:28.193939 word-search-generator-3.4.0/setup.cfg
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2021-09-14 03:36:29.000000 word-search-generator-3.4.0/setup.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.178901 word-search-generator-3.4.0/src/
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.185405 word-search-generator-3.4.0/src/word_search_generator/
+-rw-r--r--   0 jbd        (501) staff       (20)    22392 2023-06-26 21:44:11.000000 word-search-generator-3.4.0/src/word_search_generator/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)      119 2022-11-29 21:17:05.000000 word-search-generator-3.4.0/src/word_search_generator/__main__.py
+-rw-r--r--   0 jbd        (501) staff       (20)     8004 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/src/word_search_generator/cli.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1547 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/src/word_search_generator/config.py
+-rw-r--r--   0 jbd        (501) staff       (20)     6360 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/src/word_search_generator/export.py
+-rw-r--r--   0 jbd        (501) staff       (20)     7889 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/src/word_search_generator/generate.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.188415 word-search-generator-3.4.0/src/word_search_generator/mask/
+-rw-r--r--   0 jbd        (501) staff       (20)    11610 2023-03-13 18:38:34.000000 word-search-generator-3.4.0/src/word_search_generator/mask/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)     4202 2023-03-13 18:38:37.000000 word-search-generator-3.4.0/src/word_search_generator/mask/bitmap.py
+-rw-r--r--   0 jbd        (501) staff       (20)     3694 2023-03-13 18:39:21.000000 word-search-generator-3.4.0/src/word_search_generator/mask/ellipse.py
+-rw-r--r--   0 jbd        (501) staff       (20)    14385 2023-03-14 02:51:02.000000 word-search-generator-3.4.0/src/word_search_generator/mask/polygon.py
+-rw-r--r--   0 jbd        (501) staff       (20)    13001 2023-06-03 04:37:19.000000 word-search-generator-3.4.0/src/word_search_generator/mask/shapes.py
+-rw-r--r--   0 jbd        (501) staff       (20)        0 2021-09-14 03:56:24.000000 word-search-generator-3.4.0/src/word_search_generator/py.typed
+-rw-r--r--   0 jbd        (501) staff       (20)    24390 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/src/word_search_generator/utils.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.188784 word-search-generator-3.4.0/src/word_search_generator/word/
+-rw-r--r--   0 jbd        (501) staff       (20)     6881 2023-06-03 04:16:37.000000 word-search-generator-3.4.0/src/word_search_generator/word/__init__.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.186834 word-search-generator-3.4.0/src/word_search_generator.egg-info/
+-rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/PKG-INFO
+-rw-r--r--   0 jbd        (501) staff       (20)     1450 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 jbd        (501) staff       (20)        1 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       63 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/entry_points.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      180 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/requires.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       22 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/top_level.txt
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.191289 word-search-generator-3.4.0/tests/
+-rw-r--r--   0 jbd        (501) staff       (20)    15028 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/tests/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)    15204 2023-03-16 18:23:55.000000 word-search-generator-3.4.0/tests/test_Mask.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1188 2022-12-01 03:07:29.000000 word-search-generator-3.4.0/tests/test_Word.py
+-rw-r--r--   0 jbd        (501) staff       (20)    13819 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/tests/test_WordSearch.py
+-rw-r--r--   0 jbd        (501) staff       (20)     5897 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/tests/test_cli.py
+-rw-r--r--   0 jbd        (501) staff       (20)     8797 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/tests/test_export.py
+-rw-r--r--   0 jbd        (501) staff       (20)     2932 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/tests/test_generate.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1317 2023-03-16 18:06:21.000000 word-search-generator-3.4.0/tests/test_shapes.py
+-rw-r--r--   0 jbd        (501) staff       (20)     2392 2022-12-31 04:21:53.000000 word-search-generator-3.4.0/tests/test_utils.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.191771 word-search-generator-3.4.0/tools/
+-rw-r--r--   0 jbd        (501) staff       (20)      385 2023-03-16 18:09:17.000000 word-search-generator-3.4.0/tools/build_masks_output_dict.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1125 2023-01-03 03:25:46.000000 word-search-generator-3.4.0/tools/pdf_layout_testing.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.193327 word-search-generator-3.4.0/tools/sample_word_lists/
+-rw-r--r--   0 jbd        (501) staff       (20)       76 2021-08-12 01:43:53.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-10.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      173 2021-08-12 01:42:41.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-25.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       43 2021-08-12 01:41:55.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-5.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      369 2021-08-12 01:43:03.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-50.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       83 2021-08-12 02:00:51.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-junk.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      523 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/tox.ini
```

### Comparing `word-search-generator-3.3.0/.github/workflows/tests.yml` & `word-search-generator-3.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/.gitignore` & `word-search-generator-3.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/.pre-commit-config.yaml` & `word-search-generator-3.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/CHANGLOG.md` & `word-search-generator-3.4.0/CHANGLOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.4.0]
+
+### Fixed
+- `Word.offset_coordinates()`
+- Secret words correctly obey their directional constraints (by duck57). Fixes issue #42.
+
+### Changed
+
+- `show()` method now accepts the `hide_fillers` boolean argument
+    - `True` will hide all filler characters showing only the placed words (negates `solution=True`)
+
 ## [3.3.0] - 2023-05-02
 
 ### Added
 
 - New pre-built mask shapes: [Club](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Club), [Fish](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Fish), [Flower](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Flower), and [Spade](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Spade)
 - Testing for built-in masks shapes based on known output
 - 'tools/build_masks_output_dict.py' tool for generating known built-in shapes output dict for us in testing
```

### Comparing `word-search-generator-3.3.0/LICENSE` & `word-search-generator-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/PKG-INFO` & `word-search-generator-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: word-search-generator
-Version: 3.3.0
+Version: 3.4.0
 Summary: Make awesome Word Search puzzles
 Author-email: Josh Duncan <joshbduncan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/joshbduncan/word-search-generator
 Project-URL: documentation, https://github.com/joshbduncan/word-search-generator/wiki
 Project-URL: repository, https://github.com/joshbduncan/word-search-generator.git
 Project-URL: changelog, https://github.com/joshbduncan/word-search-generator/blob/main/CHANGLOG.md
```

### Comparing `word-search-generator-3.3.0/README.md` & `word-search-generator-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/pyproject.toml` & `word-search-generator-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/run` & `word-search-generator-3.4.0/run`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/__init__.py` & `word-search-generator-3.4.0/src/word_search_generator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generate Word Search puzzles with Python.
     -----------
     :copyright: (c) 2021 Josh Duncan.
     :license: MIT, see LICENSE for more details.
 """
 
 __app_name__ = "word-search"
-__version__ = "3.3.0"
+__version__ = "3.4.0"
 
 
 import json
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Set
 
 from . import export, generate, utils
@@ -180,15 +180,16 @@
     @property
     def masked(self) -> bool:
         """Puzzle masking status."""
         return bool(self.masks)
 
     @property
     def bounding_box(self) -> tuple[tuple[int, int], tuple[int, int]]:
-        """Bounding box of the active puzzle area."""
+        """Bounding box of the active puzzle area as a rectangle defined
+        by a Tuple of (top-left edge as x, y, bottom-right edge as x, y)"""
         return utils.find_bounding_box(self.mask)
 
     @property
     def cropped_puzzle(self) -> Puzzle:
         """The current puzzle state cropped to the mask."""
         min_x, min_y = self.bounding_box[0]
         max_x, max_y = self.bounding_box[1]
@@ -351,22 +352,24 @@
         else:
             self.replace_words(
                 ",".join(utils.get_random_words(count)),
                 secret=secret,
                 reset_size=reset_size,
             )
 
-    def show(self, solution: bool = False) -> None:
+    def show(self, solution: bool = False, hide_fillers: bool = False) -> None:
         """Show the current puzzle with or without the solution.
 
         Args:
             solution (bool, optional): Highlight the puzzle solution. Defaults to False.
+            hide_fillers (bool, optional): Hide all filler letters so only the solution
+                is shown. Overrides `solution`.
         """
         if self.key:
-            print(utils.format_puzzle_for_show(self, solution))
+            print(utils.format_puzzle_for_show(self, solution, hide_fillers))
         else:
             print("Empty puzzle.")
 
     def save(
         self,
         path: str | Path,
         format: str = "PDF",
@@ -407,24 +410,24 @@
 
     # *************************************************************** #
     # ******************** PROCESSING/GENERATION ******************** #
     # *************************************************************** #
 
     def _generate(self, fill_puzzle: bool = True) -> None:
         """Generate the puzzle grid."""
+        # if an empty puzzle object is created then the `random_words()` method
+        # is called set the calculate an appropriate puzzle size
+        if not self.size:
+            self.reset_size()
         self._puzzle = utils.build_puzzle(self.size, "")
         min_word_length = (
             min([len(word.text) for word in self.words]) if self.words else self.size
         )
         if self.size and self.size < min_word_length:
             raise PuzzleSizeError
-        # if an empty puzzle object is created then the `random_words()` method
-        # is called set the calculate an appropriate puzzle size
-        if not self.size:
-            self.reset_size()
         for word in self.words:
             word.remove_from_puzzle()
         if not self.mask or len(self.mask) != self.size:
             self._mask = utils.build_puzzle(self.size, ACTIVE)
         if fill_puzzle:
             self._fill_puzzle()
         if self.force_all_words and self.unplaced_hidden_words:
@@ -463,30 +466,28 @@
                 be secret. Defaults to False.
             reset_size (bool, optional): Reset the puzzle
                 size based on the updated words. Defaults to False.
         """
         self._process_input(words, "add", secret)
         if reset_size:
             self.reset_size()
-        else:
-            self._generate()
+        self._generate()
 
     def remove_words(self, words: str, reset_size: bool = False) -> None:
         """Remove words from the puzzle.
 
         Args:
             words (str): Words to remove.
             reset_size (bool, optional): Reset the puzzle
                 size based on the updated words. Defaults to False.
         """
         self._process_input(words, "remove")
         if reset_size:
             self.reset_size()
-        else:
-            self._generate()
+        self._generate()
 
     def replace_words(
         self, words: str, secret: bool = False, reset_size: bool = False
     ) -> None:
         """Replace all words from the puzzle.
 
         Args:
@@ -495,16 +496,15 @@
                 be secret. Defaults to False.
             reset_size (bool, optional): Reset the puzzle
                 size based on the updated words. Defaults to False.
         """
         self._process_input(words, "replace", secret)
         if reset_size:
             self.reset_size()
-        else:
-            self._generate()
+        self._generate()
 
     # ************************************************* #
     # ******************** MASKING ******************** #
     # ************************************************* #
 
     def apply_mask(self, mask: Mask) -> None:
         """Apply a singular mask object to the puzzle."""
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator/cli.py` & `word-search-generator-3.4.0/src/word_search_generator/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,17 +223,20 @@
         words,
         level=args.difficulty,
         size=args.size,
         secret_words=secret_words if secret_words else None,
         secret_level=args.secret_difficulty,
     )
 
-    # apply masking is specified
+    # apply masking if specified
     if args.mask:
-        puzzle.apply_mask(eval(f"shapes.{args.mask}")())
+        mask = eval(f"shapes.{args.mask}")()
+        if hasattr(mask, "min_size") and not args.size and puzzle.size < mask.min_size:
+            puzzle.size = mask.min_size
+        puzzle.apply_mask(mask)
     if args.image_mask:
         puzzle.apply_mask(Image(args.image_mask))
 
     # show the result
     if args.output or args.format:
         format = args.format if args.format else "PDF"
         path = (
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator/config.py` & `word-search-generator-3.4.0/src/word_search_generator/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,25 @@
 
 # puzzle grid settings
 ACTIVE = "*"
 INACTIVE = "#"
 
 # puzzle difficulty levels
 level_dirs = {
-    1: {Direction.E, Direction.S},
-    2: {Direction.NE, Direction.E, Direction.SE, Direction.S},
-    3: {
+    1: {  # right or down
+        Direction.E,
+        Direction.S,
+    },
+    2: {  # right-facing or down
+        Direction.NE,
+        Direction.E,
+        Direction.SE,
+        Direction.S,
+    },
+    3: {  # any direction
         Direction.N,
         Direction.NE,
         Direction.E,
         Direction.SE,
         Direction.S,
         Direction.SW,
         Direction.W,
@@ -31,16 +39,35 @@
         Direction.N,
         Direction.NE,
         Direction.SE,
         Direction.SW,
         Direction.W,
         Direction.NW,
     },
-    8: {Direction.N, Direction.E, Direction.W, Direction.S},  # no diagonals
-    7: {Direction.NE, Direction.SE, Direction.NW, Direction.SW},  # diagonals only
+    5: {  # no E
+        Direction.N,
+        Direction.NE,
+        Direction.SE,
+        Direction.S,
+        Direction.SW,
+        Direction.W,
+        Direction.NW,
+    },
+    7: {  # diagonals only
+        Direction.NE,
+        Direction.SE,
+        Direction.NW,
+        Direction.SW,
+    },
+    8: {  # no diagonals
+        Direction.N,
+        Direction.E,
+        Direction.W,
+        Direction.S,
+    },
 }
 
 # pdf export settings
 pdf_author = "Josh Duncan"
 pdf_creator = "word-search @ joshbduncan.com"
 pdf_title = "Word Search Puzzle"
 pdf_font_size_XXL = 18
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator/export.py` & `word-search-generator-3.4.0/src/word_search_generator/export.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/generate.py` & `word-search-generator-3.4.0/src/word_search_generator/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,20 +128,20 @@
         coordinates.append((row, col))
         # adjust the coordinates for the next character
         row += direction.r_move
         col += direction.c_move
     return coordinates
 
 
-def find_a_fit(ws: WordSearch, word: str, position: tuple[int, int]) -> Fit:
+def find_a_fit(ws: WordSearch, word: Word, position: tuple[int, int]) -> Fit:
     """Look for random place in the puzzle where `word` fits."""
     fits: Fits = []
     # check all directions for level
-    for d in ws.directions:
-        coords = test_a_fit(ws.puzzle, ws.mask, word, position, d)
+    for d in ws.secret_directions if word.secret else ws.directions:
+        coords = test_a_fit(ws.puzzle, ws.mask, word.text, position, d)
         if coords:
             fits.append((Direction(d).name, coords))
     # if the word fits, pick a random fit for placement
     if not fits:
         raise WordFitError
     return random.choice(fits)
 
@@ -176,15 +176,15 @@
     # no need to continue if random coordinate isn't available
     if ws.puzzle[row][col] != "" and ws.puzzle[row][col] != word.text[0]:
         raise WordFitError
     if ws.mask[row][col] == INACTIVE:
         raise WordFitError
 
     # try and find a directional fit using the starting coordinates if not INACTIVE
-    d, coords = find_a_fit(ws, word.text, (row, col))
+    d, coords = find_a_fit(ws, word, (row, col))
 
     # place word characters at fit coordinates
     previous_chars = []  # track previous to backtrack on WordFitError
     for i, char in enumerate(word.text):
         check_row = coords[i][0]
         check_col = coords[i][1]
         previous_chars.append(ws.puzzle[check_row][check_col])
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator/mask/__init__.py` & `word-search-generator-3.4.0/src/word_search_generator/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/mask/bitmap.py` & `word-search-generator-3.4.0/src/word_search_generator/mask/bitmap.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/mask/ellipse.py` & `word-search-generator-3.4.0/src/word_search_generator/mask/ellipse.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/mask/polygon.py` & `word-search-generator-3.4.0/src/word_search_generator/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/mask/shapes.py` & `word-search-generator-3.4.0/src/word_search_generator/mask/shapes.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/src/word_search_generator/utils.py` & `word-search-generator-3.4.0/src/word_search_generator/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,31 +219,50 @@
         for char in word.text:
             output[y][x] = f"\u001b[1m\u001b[31m{char}\u001b[0m"
             x += word.direction.c_move
             y += word.direction.r_move
     return output
 
 
+def hide_filler_characters(ws: WordSearch) -> Puzzle:
+    """Remove filler characters from a puzzle."""
+    output: Puzzle = copy.deepcopy(ws.puzzle)
+    word_coords = {
+        coord
+        for coords in [word.coordinates for word in ws.placed_words]
+        for coord in coords
+    }
+    for row in range(ws.size):
+        for col in range(ws.size):
+            if (col, row) not in word_coords:
+                output[col][row] = " "
+    return output
+
+
 def stringify(puzzle: Puzzle, bbox: tuple[tuple[int, int], tuple[int, int]]) -> str:
     """Convert puzzle array of nested lists into a string."""
     min_x, min_y = bbox[0]
     max_x, max_y = bbox[1]
     output = []
     offset = " " if max_x - min_x < 5 else ""
     for line in puzzle[min_y : max_y + 1]:
         output.append(
             offset + " ".join([c if c else " " for c in line[min_x : max_x + 1]])
         )
     return "\n".join(output)
 
 
-def format_puzzle_for_show(ws: WordSearch, show_solution: bool = False) -> str:
+def format_puzzle_for_show(
+    ws: WordSearch, show_solution: bool = False, hide_fillers: bool = False
+) -> str:
     word_list = get_word_list_str(ws.key)
-    # highlight solution if provided
+    # highlight solution if requested
     puzzle_list = highlight_solution(ws) if show_solution else ws.puzzle
+    # hide filler characters if requested
+    puzzle_list = hide_filler_characters(ws) if hide_fillers else puzzle_list
     # calculate header length based on cropped puzzle size to account for masks
     header_width = max(11, (ws.bounding_box[1][0] - ws.bounding_box[0][0] + 1) * 2 - 1)
     hr = "-" * header_width
     header = hr + "\n" + f"{'WORD SEARCH':^{header_width}}" + "\n" + hr
     answer_key_intro = (
         "Answer Key (*Secret Words)" if ws.placed_secret_words else "Answer Key"
     )
@@ -853,15 +872,15 @@
     "nor",
     "north",
     "not",
     "note",
     "nothing",
     "notice",
     "now",
-    "n't",
+    "nut",
     "number",
     "occur",
     "off",
     "offer",
     "office",
     "officer",
     "official",
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator/word/__init__.py` & `word-search-generator-3.4.0/src/word_search_generator/word/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         """Returns a list of the Word letter coordinates, offset
         by the puzzle bounding box.
 
         Args:
             bbox (Tuple[Tuple[int, int], Tuple[int, int]]): The current
                 puzzle bounding box.
         """
-        return [(x - bbox[0][0], y - bbox[0][1]) for x, y in self.coordinates]
+        return [(x + 1 - bbox[0][0], y + 1 - bbox[0][1]) for y, x in self.coordinates]
 
     def remove_from_puzzle(self):
         """Remove word placement details when a puzzle is reset."""
         self.start_row = None
         self.start_column = None
         self.coordinates = []
         self.direction = None
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator.egg-info/PKG-INFO` & `word-search-generator-3.4.0/src/word_search_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: word-search-generator
-Version: 3.3.0
+Version: 3.4.0
 Summary: Make awesome Word Search puzzles
 Author-email: Josh Duncan <joshbduncan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/joshbduncan/word-search-generator
 Project-URL: documentation, https://github.com/joshbduncan/word-search-generator/wiki
 Project-URL: repository, https://github.com/joshbduncan/word-search-generator.git
 Project-URL: changelog, https://github.com/joshbduncan/word-search-generator/blob/main/CHANGLOG.md
```

### Comparing `word-search-generator-3.3.0/src/word_search_generator.egg-info/SOURCES.txt` & `word-search-generator-3.4.0/src/word_search_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tests/__init__.py` & `word-search-generator-3.4.0/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Any, List
 
 from word_search_generator.mask import shapes
 
 ITERATIONS = 5
 WORDS = "dog, cat, pig, horse, donkey, turtle, goat, sheep"
+SECRET_WORDS = "rabbit, mule, bunny, ram, kitten, puppy, foal"
+# "tortoise" not included in SECRET_WORDS because it is 8 characters long
+# everything else tops out at 6
 
 # Put all shape masks into a list for use in testing
 BUILTIN_MASK_SHAPES_OBJECTS: List[Any] = []
 for shape in shapes.BUILTIN_MASK_SHAPES:
     mask = eval(f"shapes.{shape}")()
     BUILTIN_MASK_SHAPES_OBJECTS.append(mask)
```

### Comparing `word-search-generator-3.3.0/tests/test_Mask.py` & `word-search-generator-3.4.0/tests/test_Mask.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tests/test_Word.py` & `word-search-generator-3.4.0/tests/test_Word.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tests/test_WordSearch.py` & `word-search-generator-3.4.0/tests/test_WordSearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 import pathlib
 import random
+from typing import Set
 
 import pytest
 
 from word_search_generator import (
     Key,
     MissingWordError,
     Puzzle,
     PuzzleSizeError,
     WordSearch,
     config,
     utils,
 )
 from word_search_generator.config import level_dirs
 from word_search_generator.mask.polygon import Rectangle
-from word_search_generator.utils import get_random_words
 from word_search_generator.word import Direction, Word
 
-from . import BUILTIN_MASK_SHAPES_OBJECTS, ITERATIONS, WORDS
+from . import BUILTIN_MASK_SHAPES_OBJECTS, ITERATIONS, SECRET_WORDS, WORDS
 
 
 def check_chars(puzzle, word):
     row, col = word.position
     for c in word.text:
         if c != puzzle[row][col]:
             return False
@@ -274,21 +274,21 @@
     capture1 = capsys.readouterr()
     ws.show(True)
     capture2 = capsys.readouterr()
     assert capture1.out == capture2.out
 
 
 def test_json_output_property_for_puzzle():
-    words = ",".join(get_random_words(10))
+    words = ",".join(utils.get_random_words(10))
     ws = WordSearch(words, level=3)
     assert json.loads(ws.json)["puzzle"] == ws.puzzle
 
 
 def test_json_output_property_for_key():
-    words = ",".join(get_random_words(10))
+    words = ",".join(utils.get_random_words(10))
     p = WordSearch(words, level=3)
     json_key = json.loads(p.json)["key"]
     for word, info in json_key.items():
         pos = (info["start_row"], info["start_col"])
         assert pos == p.key[word]["start"]
 
 
@@ -300,15 +300,15 @@
 def test_input_including_palindrome():
     ws = WordSearch(WORDS + ", level")
     assert len(ws.words) == 8
 
 
 def test_for_empty_spaces():
     for _ in range(ITERATIONS * 20):
-        words = ",".join(get_random_words(10))
+        words = ",".join(utils.get_random_words(10))
         ws = WordSearch(words, level=3)
         flat = [item for sublist in ws.puzzle for item in sublist]
         assert ws.size * ws.size == len(flat)
 
 
 def test_puzzle_with_secret_words():
     ws = WordSearch(WORDS, secret_words=WORDS + ", dewlap")
@@ -498,7 +498,47 @@
     assert all(results)
 
 
 def test_puzzle_size_error():
     p = WordSearch("abracadabra")
     with pytest.raises(PuzzleSizeError):
         p.size = 5
+
+
+def test_hide_fillers():
+    results = []
+    for _ in range(ITERATIONS):
+        p = WordSearch(size=random.randint(21, 35))
+        p.random_words(random.randint(5, 21))
+        mask = random.choice(BUILTIN_MASK_SHAPES_OBJECTS)
+        if mask:
+            p.apply_mask(mask)
+        hidden_fillers = utils.hide_filler_characters(p)
+        chars: Set[str] = set()
+        for word in p.placed_words:
+            chars.update(hidden_fillers[y][x] for y, x in word.coordinates)
+        results.append(" " not in chars)
+    assert all(results)
+
+
+def test_solution_plus_hide_fillers():
+    results = []
+    for _ in range(ITERATIONS):
+        p = WordSearch(size=random.randint(21, 35))
+        p.random_words(random.randint(5, 21))
+        mask = random.choice(BUILTIN_MASK_SHAPES_OBJECTS)
+        if mask:
+            p.apply_mask(mask)
+        chars = {c for chars in p.puzzle for c in chars}
+        results.append("\x1b" not in chars)
+    assert all(results)
+
+
+def test_word_directions():
+    """
+    Hidden words can go NE, E, SE, or S.
+    Secret words go on diagonals.
+    Do they all obey the restriction rules?
+    """
+    p = WordSearch(WORDS, secret_words=SECRET_WORDS, secret_level=7)
+    assert all(w.direction in p.directions for w in p.placed_hidden_words)
+    assert all(w.direction in p.secret_directions for w in p.placed_secret_words)
```

### Comparing `word-search-generator-3.3.0/tests/test_cli.py` & `word-search-generator-3.4.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,19 @@
 
 
 def test_mask():
     result = subprocess.run("word-search -r 5 -s 21 -m Triangle", shell=True)
     assert result.returncode == 0
 
 
+def test_shape_mask_min_size():
+    result = subprocess.run("word-search -r 1 -m Club", shell=True)
+    assert result.returncode == 0
+
+
 def test_invalid_mask():
     result = subprocess.run("word-search -r 5 -s 21 -m Heptakaideka", shell=True)
     assert result.returncode == 2
 
 
 def test_image_mask(tmp_path):
     name = "test_image.jpg"
```

### Comparing `word-search-generator-3.3.0/tests/test_export.py` & `word-search-generator-3.4.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tests/test_generate.py` & `word-search-generator-3.4.0/tests/test_generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from word_search_generator import WordSearch
-from word_search_generator.config import max_puzzle_words
+from word_search_generator.config import level_dirs, max_puzzle_words
 from word_search_generator.generate import no_duped_words
 from word_search_generator.utils import get_random_words
 from word_search_generator.word import Direction, Word, Wordlist
 
 
 def setup_words():
     BAT = Word("bat")
@@ -91,7 +91,19 @@
 
 
 def test_too_many_secret_words():
     p = WordSearch(size=50)
     p.random_words(100)
     p.random_words(100, action="ADD", secret=True)
     assert len(p.placed_words) <= max_puzzle_words
+
+
+def test_secret_word_directions():
+    words = "cat bat rat"
+    level = 1  # right or down
+    secret_words = "pig dog fox"
+    secret_level = 7  # diagonals only
+    p = WordSearch(
+        words, level=level, secret_words=secret_words, secret_level=secret_level
+    )
+    for w in p.placed_secret_words:
+        assert w.direction in level_dirs[secret_level]
```

### Comparing `word-search-generator-3.3.0/tests/test_shapes.py` & `word-search-generator-3.4.0/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tests/test_utils.py` & `word-search-generator-3.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tools/pdf_layout_testing.py` & `word-search-generator-3.4.0/tools/pdf_layout_testing.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.3.0/tox.ini` & `word-search-generator-3.4.0/tox.ini`

 * *Files identical despite different names*

