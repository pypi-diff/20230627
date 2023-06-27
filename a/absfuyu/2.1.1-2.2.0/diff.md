# Comparing `tmp/absfuyu-2.1.1.tar.gz` & `tmp/absfuyu-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-ki_676fk\absfuyu-2.1.1.tar", last modified: Thu Jun 15 08:11:27 2023, max compression
+gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-_vasoj_t\absfuyu-2.2.0.tar", last modified: Tue Jun 27 11:09:14 2023, max compression
```

## Comparing `absfuyu-2.1.1.tar` & `absfuyu-2.2.0.tar`

### file list

```diff
@@ -1,110 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/
--rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.1.1/LICENSE
--rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3836 2023-06-15 08:11:27.000000 absfuyu-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.1.1/README.md
--rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.1.1/extra_requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.000000 absfuyu-2.1.1/images/
--rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.1.1/images/repository-image-crop.png
--rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0     1360 2023-06-15 08:11:27.000000 absfuyu-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu/
--rw-rw-rw-   0        0        0     1004 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/__init__.py
--rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/__main__.py
--rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/calculation.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/code_red/
--rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-2.1.1/src/absfuyu/code_red/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/collections/
--rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.1.1/src/absfuyu/collections/__init__.py
--rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/collections/content.py
--rw-rw-rw-   0        0        0    20864 2023-06-15 07:26:41.000000 absfuyu-2.1.1/src/absfuyu/collections/data_extension.py
--rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/collections/generator.py
--rw-rw-rw-   0        0        0     5822 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/collections/human.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/config/
--rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/config/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-15 08:11:14.000000 absfuyu-2.1.1/src/absfuyu/config/config.json
--rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/config/config2.py
--rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.1.1/src/absfuyu/config/template.json
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/contrib/
--rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.1.1/src/absfuyu/contrib/__init__.py
--rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/contrib/basic_lunar_calendar.py
--rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.1.1/src/absfuyu/contrib/color_extract.py
--rw-rw-rw-   0        0        0     3313 2023-06-15 07:52:56.000000 absfuyu-2.1.1/src/absfuyu/core.py
--rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/everything.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/
--rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.1.1/src/absfuyu/extensions/__init__.py
--rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.1.1/src/absfuyu/extensions/beautiful.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/
--rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/WGS.py
--rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/__init__.py
--rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/horoscope.py
--rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/password_hash.py
--rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/pkglib.py
--rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/primo_cal.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/
--rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/__init__.py
--rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/rebrandly.py
--rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/tarot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/extra/
--rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.1.1/src/absfuyu/extensions/extra/__init__.py
--rw-rw-rw-   0        0        0     6812 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/extensions/extra/data_analysis.py
--rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/fun.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/game/
--rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.1.1/src/absfuyu/game/__init__.py
--rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/game/sudoku.py
--rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.1.1/src/absfuyu/game/tictactoe.py
--rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/game/wordle.py
--rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.1.1/src/absfuyu/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/
--rw-rw-rw-   0        0        0     3043 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/__init__.py
--rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/chemistry.json
--rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/dummy.dat
--rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/punishment_windows.dat
--rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/tarot.json
--rw-rw-rw-   0        0        0     5882 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/sort.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/tools/
--rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/__init__.py
--rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/converter.py
--rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.1.1/src/absfuyu/tools/keygen.py
--rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/obfuscator.py
--rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/stats.py
--rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/web.py
--rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/unused.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/util/
--rw-rw-rw-   0        0        0     2396 2023-06-09 13:47:13.000000 absfuyu-2.1.1/src/absfuyu/util/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/api.py
--rw-rw-rw-   0        0        0     2366 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/json_method.py
--rw-rw-rw-   0        0        0     5512 2023-06-15 08:10:16.000000 absfuyu-2.1.1/src/absfuyu/util/path.py
--rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/performance.py
--rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.1.1/src/absfuyu/util/pkl.py
--rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/zipped.py
--rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.1.1/src/absfuyu/version.py
--rw-rw-rw-   0        0        0     9951 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/version2.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu.egg-info/
--rw-rw-rw-   0        0        0     3836 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2639 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1266 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/tests/
--rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_DictKai.py
--rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_Generator.py
--rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_IntNumber.py
--rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_ListKai.py
--rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_Text.py
--rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_api.py
--rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.1.1/tests/test_beautiful.py
--rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.1.1/tests/test_config.py
--rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_converter.py
--rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.1.1/tests/test_everything.py
--rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.1.1/tests/test_extensions.py
--rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.1.1/tests/test_fun.py
--rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_json_method.py
--rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_obfuscator.py
--rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_path.py
--rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.1.1/tests/test_pkg_data.py
--rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/
+-rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3836 2023-06-27 11:09:14.000000 absfuyu-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.2.0/README.md
+-rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.2.0/extra_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/images/
+-rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.2.0/images/repository-image-crop.png
+-rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.2.0/requirements.txt
+-rw-rw-rw-   0        0        0     1360 2023-06-27 11:09:14.000000 absfuyu-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/
+-rw-rw-rw-   0        0        0      941 2023-06-27 11:01:33.000000 absfuyu-2.2.0/src/absfuyu/__init__.py
+-rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/__main__.py
+-rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/calculation.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/collections/
+-rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.2.0/src/absfuyu/collections/__init__.py
+-rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/collections/content.py
+-rw-rw-rw-   0        0        0    22151 2023-06-16 11:44:52.000000 absfuyu-2.2.0/src/absfuyu/collections/data_extension.py
+-rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/collections/generator.py
+-rw-rw-rw-   0        0        0     5822 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/collections/human.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/config/
+-rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.2.0/src/absfuyu/config/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-27 11:08:57.000000 absfuyu-2.2.0/src/absfuyu/config/config.json
+-rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/config/config2.py
+-rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.2.0/src/absfuyu/config/template.json
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/contrib/
+-rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.2.0/src/absfuyu/contrib/__init__.py
+-rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/contrib/basic_lunar_calendar.py
+-rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.2.0/src/absfuyu/contrib/color_extract.py
+-rw-rw-rw-   0        0        0     3313 2023-06-15 07:52:56.000000 absfuyu-2.2.0/src/absfuyu/core.py
+-rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/everything.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/
+-rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.2.0/src/absfuyu/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.2.0/src/absfuyu/extensions/beautiful.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/
+-rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/WGS.py
+-rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/__init__.py
+-rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/horoscope.py
+-rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/password_hash.py
+-rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/pkglib.py
+-rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/primo_cal.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/
+-rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/__init__.py
+-rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/rebrandly.py
+-rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/tarot.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/extra/
+-rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.2.0/src/absfuyu/extensions/extra/__init__.py
+-rw-rw-rw-   0        0        0     7416 2023-06-27 10:59:07.000000 absfuyu-2.2.0/src/absfuyu/extensions/extra/data_analysis.py
+-rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/fun.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/game/
+-rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.2.0/src/absfuyu/game/__init__.py
+-rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.2.0/src/absfuyu/game/sudoku.py
+-rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.2.0/src/absfuyu/game/tictactoe.py
+-rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.2.0/src/absfuyu/game/wordle.py
+-rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.2.0/src/absfuyu/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/
+-rw-rw-rw-   0        0        0     3016 2023-06-27 11:00:53.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/__init__.py
+-rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/chemistry.json
+-rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/tarot.json
+-rw-rw-rw-   0        0        0     5848 2023-06-25 13:09:10.000000 absfuyu-2.2.0/src/absfuyu/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/tools/
+-rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/converter.py
+-rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.2.0/src/absfuyu/tools/keygen.py
+-rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/obfuscator.py
+-rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/stats.py
+-rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/web.py
+-rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/unused.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/util/
+-rw-rw-rw-   0        0        0     2396 2023-06-09 13:47:13.000000 absfuyu-2.2.0/src/absfuyu/util/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/api.py
+-rw-rw-rw-   0        0        0     2366 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/json_method.py
+-rw-rw-rw-   0        0        0     5512 2023-06-15 08:10:16.000000 absfuyu-2.2.0/src/absfuyu/util/path.py
+-rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/performance.py
+-rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.2.0/src/absfuyu/util/pkl.py
+-rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/zipped.py
+-rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.2.0/src/absfuyu/version.py
+-rw-rw-rw-   0        0        0     9951 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/version2.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2531 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1266 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/tests/
+-rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_DictKai.py
+-rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_Generator.py
+-rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_IntNumber.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_ListKai.py
+-rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_Text.py
+-rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_api.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.2.0/tests/test_beautiful.py
+-rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.2.0/tests/test_config.py
+-rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_converter.py
+-rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.2.0/tests/test_everything.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.2.0/tests/test_extensions.py
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.2.0/tests/test_fun.py
+-rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_json_method.py
+-rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_obfuscator.py
+-rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_path.py
+-rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.2.0/tests/test_pkg_data.py
+-rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_util.py
```

### Comparing `absfuyu-2.1.1/LICENSE` & `absfuyu-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/PKG-INFO` & `absfuyu-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.1.1
+Version: 2.2.0
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -18,36 +18,36 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: beautiful
 Provides-Extra: rich
+Provides-Extra: dev
 Provides-Extra: click
-Provides-Extra: cli
 Provides-Extra: extra
+Provides-Extra: cli
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
 Provides-Extra: pipx
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: autoimport
 Provides-Extra: fixers
+Provides-Extra: autoimport
 Provides-Extra: black
 Provides-Extra: pytest
 Provides-Extra: test
 Provides-Extra: tox
 Provides-Extra: sphinx
 Provides-Extra: sphinx_rtd_theme
 Provides-Extra: python-dateutil
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 2.1.1 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.2.0 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-beautiful Provides-Extra: rich Provides-Extra: click Provides-Extra: cli
-Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
+Description-Content-Type: text/markdown Provides-Extra: beautiful Provides-
+Extra: rich Provides-Extra: dev Provides-Extra: click Provides-Extra: extra
+Provides-Extra: cli Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
+fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.1.1/README.md` & `absfuyu-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/extra_requirements.txt` & `absfuyu-2.2.0/extra_requirements.txt`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/images/repository-image-crop.png` & `absfuyu-2.2.0/images/repository-image-crop.png`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/setup.cfg` & `absfuyu-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/setup.py` & `absfuyu-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/__init__.py` & `absfuyu-2.2.0/src/absfuyu/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,12 +45,7 @@
 from . import calculation as cal
 from . import util
 
 
 # config
 # from . import config as __config
 # __config.welcome()
-
-
-# luckgod
-from . import code_red as __red
-__red.luckgod()
```

### Comparing `absfuyu-2.1.1/src/absfuyu/__main__.py` & `absfuyu-2.2.0/src/absfuyu/__main__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/calculation.py` & `absfuyu-2.2.0/src/absfuyu/calculation.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/collections/__init__.py` & `absfuyu-2.2.0/src/absfuyu/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/collections/content.py` & `absfuyu-2.2.0/src/absfuyu/collections/content.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/collections/data_extension.py` & `absfuyu-2.2.0/src/absfuyu/collections/data_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Absfuyu: Data extension
 ---
 Extension for data type such as `list`, `str`, ...
 
-Version: 1.2.0
-Date updated: 15/06/2023 (dd/mm/yyyy)
+Version: 1.3.0
+Date updated: 16/06/2023 (dd/mm/yyyy)
 
 Features:
 - Text
 - ListKai
 - DictKai
 - IntNumber
 """
@@ -21,23 +21,23 @@
     "ListKai", "DictKai"
 ]
 
 
 # Library
 ###########################################################################
 from collections import Counter
-from itertools import accumulate, groupby
+from itertools import accumulate, chain, groupby
 import math
 import operator
 import random
-from typing import Union
+from typing import Any, Dict, List, Union
 
 from absfuyu.collections.generator import Generator, Charset
 from absfuyu.logger import logger, log_debug
-from absfuyu.util import set_min_max
+from absfuyu.util import set_min, set_min_max
 
 
 # Class
 ###########################################################################
 class Text(str):
     """
     `str` extension
@@ -618,15 +618,17 @@
             logger.debug(out)
             return out
         else:
             logger.debug("List empty!")
             return None
     
     def len_items(self):
-        """`len()` for every item in list"""
+        """
+        `len()` for every item in `list[str]`
+        """
         out = ListKai([len(str(x)) for x in self])
         # out = ListKai(map(lambda x: len(str(x)), self))
         logger.debug(out)
         return out
 
     def mean_len(self):
         """Average length of every item"""
@@ -643,28 +645,71 @@
         """Remove duplicates"""
         return __class__(set(self))
     
     def group_by_unique(self):
         """
         Group duplicated elements into list
         
-        Example:
-        ---
+        Example
+        -------
+
         >>> test = ListKai([1, 2, 3, 1, 3, 3, 2])
         >>> test.group_by_unique()
         [[1, 1], [2, 2], [3, 3, 3]]
         """
         # Old
         # out = self.sorts().slice_points(self.freq(appear_increment=True))
         # return __class__(out[:-1])
 
         # New
         temp = groupby(self.sorts())
         return __class__([list(g) for _, g in temp])
 
+    def group_by_pair_value(self, max_loop: int = 3) -> List[list]:
+        """
+        Assume each `list` in `list` is a pair value, 
+        returns a `list` contain all paired value
+
+        max_loop: times to run functions (minimum: 3)
+
+        Example
+        -------
+
+        >>> [[1, 2], [2, 3], [4, 3], [5, 6]]
+        [[1, 2, 3, 4], [5, 6]]
+
+        >>> [[8, 3], [4, 6], [6, 3], [5, 2], [7, 2]]
+        [[8, 3, 4, 6], [2, 5, 7]]
+
+        >>> [["a", 4], ["b", 4], [5, "c"]]
+        [["a", "b", 4], ["c", 5]]
+        """
+
+        iter = self.copy()
+
+        # Init loop
+        for _ in range(set_min(max_loop, min_value=3)):
+
+            temp: Dict[Any, list] = {}
+            # Make dict{key: all `item` that contains `key`}
+            for item in iter:
+                for x in item:
+                    if temp.get(x, None) is None:
+                        temp[x] = [item]
+                    else:
+                        temp[x].append(item)
+
+            # Flatten dict.values
+            for k, v in temp.items():
+                temp[k] = list(set(chain(*v)))
+            
+            iter = list(temp.values())
+
+        return list(x for x, _ in groupby(iter))
+
 
 class DictKai(dict):
     """
     `dict` extension
     """
     def analyze(self):
         """
```

### Comparing `absfuyu-2.1.1/src/absfuyu/collections/generator.py` & `absfuyu-2.2.0/src/absfuyu/collections/generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/collections/human.py` & `absfuyu-2.2.0/src/absfuyu/collections/human.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/config/__init__.py` & `absfuyu-2.2.0/src/absfuyu/config/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/config/config.json` & `absfuyu-2.2.0/src/absfuyu/config/template.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "{'major': 1, 'patch': 4}"}*

```diff
@@ -18,14 +18,14 @@
         "test": {
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
-        "major": 2,
+        "major": 1,
         "minor": 1,
-        "patch": 1,
+        "patch": 4,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.1.1/src/absfuyu/config/config2.py` & `absfuyu-2.2.0/src/absfuyu/config/config2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/config/template.json` & `absfuyu-2.2.0/src/absfuyu/config/config.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925%*

 * *Differences: {"'version'": "{'major': 2, 'minor': 2, 'patch': 0}"}*

```diff
@@ -18,14 +18,14 @@
         "test": {
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
-        "major": 1,
-        "minor": 1,
-        "patch": 4,
+        "major": 2,
+        "minor": 2,
+        "patch": 0,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.1.1/src/absfuyu/contrib/basic_lunar_calendar.py` & `absfuyu-2.2.0/src/absfuyu/contrib/basic_lunar_calendar.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/contrib/color_extract.py` & `absfuyu-2.2.0/src/absfuyu/contrib/color_extract.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/core.py` & `absfuyu-2.2.0/src/absfuyu/core.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/everything.py` & `absfuyu-2.2.0/src/absfuyu/everything.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/beautiful.py` & `absfuyu-2.2.0/src/absfuyu/extensions/beautiful.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/WGS.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/WGS.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/horoscope.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/horoscope.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/password_hash.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/pkglib.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/pkglib.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/primo_cal.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/primo_cal.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/rebrandly.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/rebrandly.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/dev/tarot.py` & `absfuyu-2.2.0/src/absfuyu/extensions/dev/tarot.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-2.2.0/src/absfuyu/extensions/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/extensions/extra/data_analysis.py` & `absfuyu-2.2.0/src/absfuyu/extensions/extra/data_analysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,56 @@
 """
-ABSFUYU-EXTRA: DATA ANALYSIS
--------------
-"""
+Absfuyu: Data Analysis
+---
+Extension for `pd.DataFrame`
 
+Version: 2.0.0
+Date updated: 15/06/2023 (dd/mm/yyyy)
+"""
 
 
 # Library
-##############################################################
-import random as __random
-import itertools as __itertools
-__EXTRA_MODE = False
-__ERROR_MSG = "This feature is in absfuyu[extra] package"
-try:
-    import pandas as __pd
-    import numpy as __np
-    import matplotlib.pyplot as __plt
-    from scipy import stats as __stats
-except ImportError:
-    from absfuyu.config import show_cfg as __aie
-    if __aie("auto-install-extra", raw=True):
-        __cmd: str = "python -m pip install -U absfuyu[extra]".split()
-        from subprocess import run as __run
-        __run(__cmd)
-    else:
-        raise SystemExit(__ERROR_MSG)
-else:
-    __EXTRA_MODE = True
+###########################################################################
+import random
+import itertools
+from typing import Union
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+from scipy import stats
 
 
 
 # Function
-##############################################################
-def isloaded():
-    try:
-        if __EXTRA_MODE:
-            return True
-        else:
-            return False
-    except:
-        return True
-
-def __validate():
-    if not __EXTRA_MODE:
-        raise SystemExit(__ERROR_MSG)
-
-
-def summary(data):
+###########################################################################
+def summary(data: Union[list, np.ndarray]):
     """
     Quick summary of data
     
     data : np.ndarray | list
     """
-
-    __validate()
         
-    if not isinstance(data, __np.ndarray):
-        data = __np.array(data)
+    if not isinstance(data, np.ndarray):
+        data = np.array(data)
 
     output = {
         "Observations": len(data),
-        "Mean": __np.mean(data),
-        "Median": __np.median(data),
-        "Mode": __stats.mode(data)[0][0],
-        "Standard deviation": __np.std(data),
-        "Variance": __np.var(data),
+        "Mean": np.mean(data),
+        "Median": np.median(data),
+        "Mode": stats.mode(data)[0][0],
+        "Standard deviation": np.std(data),
+        "Variance": np.var(data),
         "Max": max(data),
         "Min": min(data),
         "Percentiles": {
-            "1st Quartile": __np.quantile(data, 0.25),
-            "2nd Quartile": __np.quantile(data, 0.50),
-            "3rd Quartile": __np.quantile(data, 0.75),
-            "IQR": __stats.iqr(data),
+            "1st Quartile": np.quantile(data, 0.25),
+            "2nd Quartile": np.quantile(data, 0.50),
+            "3rd Quartile": np.quantile(data, 0.75),
+            "IQR": stats.iqr(data),
         },
     }
     return output
 
 
 def mplt_fmt_str(
         marker = None,
@@ -175,21 +151,21 @@
             # "w",
         ]
     else:
         color_list = color
     
     if not random:
         fmt_str = [marker_list, linestyle_list, color_list]
-        fmt_str_comb = ["".join(x) for x in list(__itertools.product(*fmt_str))]
+        fmt_str_comb = ["".join(x) for x in list(itertools.product(*fmt_str))]
         return fmt_str_comb
 
     format_string = [
-        __random.choice(marker_list),
-        __random.choice(linestyle_list),
-        __random.choice(color_list),
+        random.choice(marker_list),
+        random.choice(linestyle_list),
+        random.choice(color_list),
     ]
 
     if raw:
         return format_string
 
     if alt:
         return "".join([format_string[2], format_string[0], format_string[1]])
@@ -217,63 +193,111 @@
             if error_count > max_error:
                 break
     
     # Output
     return fs
 
 
-def divide_dataframe(df: __pd.DataFrame, by: str) -> list:
+def divide_dataframe(df: pd.DataFrame, by: str) -> list:
     """
     Divide df into a list of df
     """
     divided = [y for _, y in df.groupby(by)]
     # divided[0] # this is the first separated df
     # divided[len(divided)-1] # this is the last separated df
     return divided
 
 
-def delta_date(df: __pd.DataFrame, date_field: str, col_name: str="delta_date"):
+def delta_date(df: pd.DataFrame, date_field: str, col_name: str="delta_date"):
     """
     Calculate date interval between row
     """
     dated = df[date_field].to_list()
     cal = []
     for i in range(len(dated)):
         if i==0:
             cal.append(dated[i]-dated[i])
         else:
             cal.append(dated[i]-dated[i-1])
     df[col_name] = [x.days for x in cal]
     return df
 
 
-def get_unique(df: __pd.DataFrame, col:str):
-    """
-    Return a list of unique values in a column
-    """
-    return list(df[col].unique())
-
 
-def modify_date(df: __pd.DataFrame, date_col: str):
+def modify_date(df: pd.DataFrame, date_col: str):
     """
     Add date, week, and year column for date_col
     """
-    df["Date"] = __pd.to_datetime(df[date_col])
+    df["Date"] = pd.to_datetime(df[date_col])
     df["Week"] = df["Date"].dt.isocalendar().week
     df["Year"] = df["Date"].dt.isocalendar().year
     return df
 
 
-def equalize_df(data: dict, fillna = __np.nan):
+def equalize_df(data: dict, fillna = np.nan):
     """
     Make all list in dict have equal length to make pd.DataFrame
     """
     max_len = 0
     for _, v in data.items():
         if len(v) >= max_len:
             max_len = len(v)
     for _, v in data.items():
         if len(v) < max_len:
             missings = max_len-len(v)
             for _ in range(missings):
                 v.append(fillna)
-    return data
+    return data
+
+
+
+# Class
+###########################################################################
+class MatplotlibFormatString:
+    pass
+
+
+class DataFrameKai(pd.DataFrame):
+    def get_unique(self, col: str):
+        """
+        Return a list of unique values in a column
+        """
+        return list(self[col].unique())
+    
+    def convert_to_SeriesKai(self):
+        pass
+
+    def summary(self, col: str):
+        """
+        Quick summary of data
+        """
+        data = self[col]
+            
+        if not isinstance(data, np.ndarray):
+            data = np.array(data)
+
+        output = {
+            "Observations": len(data),
+            "Mean": np.mean(data),
+            "Median": np.median(data),
+            "Mode": stats.mode(data)[0][0],
+            "Standard deviation": np.std(data),
+            "Variance": np.var(data),
+            "Max": max(data),
+            "Min": min(data),
+            "Percentiles": {
+                "1st Quartile": np.quantile(data, 0.25),
+                "2nd Quartile": np.quantile(data, 0.50),
+                "3rd Quartile": np.quantile(data, 0.75),
+                "IQR": stats.iqr(data),
+            },
+        }
+        return output
+
+
+class SeriesKai(pd.Series):
+    pass
+
+# Run
+###########################################################################
+if __name__ == "__main__":
+    pass
```

### Comparing `absfuyu-2.1.1/src/absfuyu/fun.py` & `absfuyu-2.2.0/src/absfuyu/fun.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/game/__init__.py` & `absfuyu-2.2.0/src/absfuyu/game/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/game/sudoku.py` & `absfuyu-2.2.0/src/absfuyu/game/sudoku.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/game/tictactoe.py` & `absfuyu-2.2.0/src/absfuyu/game/tictactoe.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/game/wordle.py` & `absfuyu-2.2.0/src/absfuyu/game/wordle.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/logger.py` & `absfuyu-2.2.0/src/absfuyu/logger.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/pkg_data/__init__.py` & `absfuyu-2.2.0/src/absfuyu/pkg_data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     else:
         return None
 
 
 # Class
 ###########################################################################
 class DataList:
-    DUMMY = "dummy.dat"
-    PWIN = "punishment_windows.dat"
+    DUMMY = None
+    PWIN = None
 
 
 class PkgData:
     """Package data maker/loader"""
     def __init__(self, data_name: str) -> None:
         self.name = data_name
```

### Comparing `absfuyu-2.1.1/src/absfuyu/pkg_data/chemistry.json` & `absfuyu-2.2.0/src/absfuyu/pkg_data/chemistry.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/pkg_data/tarot.json` & `absfuyu-2.2.0/src/absfuyu/pkg_data/tarot.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/sort.py` & `absfuyu-2.2.0/src/absfuyu/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Absfuyu: Sort
 ---
 Sort Module
 
-Version: 1.2.0
-Last update: 25/05/2023 (mm/dd/yyyy)
+Version: 1.2.1
+Last update: 25/06/2023 (mm/dd/yyyy)
 
 Contain:
 - selection_sort
 - insertion_sort
 """
 
 
@@ -22,17 +22,15 @@
 
 
 # Library
 ###########################################################################
 from collections import Counter, namedtuple
 from itertools import accumulate
 import operator
-from typing import Dict as __Dict
-from typing import List as __List
-from typing import Union as __Union
+from typing import Dict as __Dict, List as __List, Union as __Union
 
 from absfuyu.logger import logger
 
 
 # Functions
 ###########################################################################
 def selection_sort(lst: list, reverse: bool = False) -> list:
@@ -213,15 +211,15 @@
 def binary_search(iterable: list, key):
     """
     Returns the position of key in the list if found, -1 otherwise.
 
     List must be sorted.
     """
     left = 0
-    right = len(list) - 1
+    right = len(iterable) - 1
     while left <= right:
         middle = (left + right) // 2
         
         if iterable[middle] == key:
             return middle
         if iterable[middle] > key:
             right = middle - 1
```

### Comparing `absfuyu-2.1.1/src/absfuyu/tools/converter.py` & `absfuyu-2.2.0/src/absfuyu/tools/converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/tools/keygen.py` & `absfuyu-2.2.0/src/absfuyu/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/tools/obfuscator.py` & `absfuyu-2.2.0/src/absfuyu/tools/obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/tools/stats.py` & `absfuyu-2.2.0/src/absfuyu/tools/stats.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/tools/web.py` & `absfuyu-2.2.0/src/absfuyu/tools/web.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/unused.py` & `absfuyu-2.2.0/src/absfuyu/unused.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/__init__.py` & `absfuyu-2.2.0/src/absfuyu/util/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/api.py` & `absfuyu-2.2.0/src/absfuyu/util/api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/json_method.py` & `absfuyu-2.2.0/src/absfuyu/util/json_method.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/path.py` & `absfuyu-2.2.0/src/absfuyu/util/path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/performance.py` & `absfuyu-2.2.0/src/absfuyu/util/performance.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/pkl.py` & `absfuyu-2.2.0/src/absfuyu/util/pkl.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/util/zipped.py` & `absfuyu-2.2.0/src/absfuyu/util/zipped.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/version.py` & `absfuyu-2.2.0/src/absfuyu/version.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu/version2.py` & `absfuyu-2.2.0/src/absfuyu/version2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/src/absfuyu.egg-info/PKG-INFO` & `absfuyu-2.2.0/src/absfuyu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.1.1
+Version: 2.2.0
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -18,36 +18,36 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: beautiful
 Provides-Extra: rich
+Provides-Extra: dev
 Provides-Extra: click
-Provides-Extra: cli
 Provides-Extra: extra
+Provides-Extra: cli
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
 Provides-Extra: pipx
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: autoimport
 Provides-Extra: fixers
+Provides-Extra: autoimport
 Provides-Extra: black
 Provides-Extra: pytest
 Provides-Extra: test
 Provides-Extra: tox
 Provides-Extra: sphinx
 Provides-Extra: sphinx_rtd_theme
 Provides-Extra: python-dateutil
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 2.1.1 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.2.0 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-beautiful Provides-Extra: rich Provides-Extra: click Provides-Extra: cli
-Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
+Description-Content-Type: text/markdown Provides-Extra: beautiful Provides-
+Extra: rich Provides-Extra: dev Provides-Extra: click Provides-Extra: extra
+Provides-Extra: cli Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
+fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.1.1/src/absfuyu.egg-info/SOURCES.txt` & `absfuyu-2.2.0/src/absfuyu.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 src/absfuyu/version2.py
 src/absfuyu.egg-info/PKG-INFO
 src/absfuyu.egg-info/SOURCES.txt
 src/absfuyu.egg-info/dependency_links.txt
 src/absfuyu.egg-info/entry_points.txt
 src/absfuyu.egg-info/requires.txt
 src/absfuyu.egg-info/top_level.txt
-src/absfuyu/code_red/__init__.py
 src/absfuyu/collections/__init__.py
 src/absfuyu/collections/content.py
 src/absfuyu/collections/data_extension.py
 src/absfuyu/collections/generator.py
 src/absfuyu/collections/human.py
 src/absfuyu/config/__init__.py
 src/absfuyu/config/config.json
@@ -52,16 +51,14 @@
 src/absfuyu/extensions/extra/data_analysis.py
 src/absfuyu/game/__init__.py
 src/absfuyu/game/sudoku.py
 src/absfuyu/game/tictactoe.py
 src/absfuyu/game/wordle.py
 src/absfuyu/pkg_data/__init__.py
 src/absfuyu/pkg_data/chemistry.json
-src/absfuyu/pkg_data/dummy.dat
-src/absfuyu/pkg_data/punishment_windows.dat
 src/absfuyu/pkg_data/tarot.json
 src/absfuyu/tools/__init__.py
 src/absfuyu/tools/converter.py
 src/absfuyu/tools/keygen.py
 src/absfuyu/tools/obfuscator.py
 src/absfuyu/tools/stats.py
 src/absfuyu/tools/web.py
```

### Comparing `absfuyu-2.1.1/src/absfuyu.egg-info/requires.txt` & `absfuyu-2.2.0/src/absfuyu.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 [:python_version == "3.7"]
 typing_extensions>=3.7.4
 
 [LunarCalendar]
 LunarCalendar>=0.0.9
 
 [all]
+tox>=3.24.5
+scipy
+pandas
+LunarCalendar>=0.0.9
+unidecode
 autoimport
-matplotlib
-sphinx_rtd_theme
 virtualenv>=20.13.0
-pipx
 pytest>=6.2.5
-LunarCalendar>=0.0.9
-tox>=3.24.5
+black>=22.1.0
+build
 sphinx
-scipy
+sphinx_rtd_theme
+wheel
+rich
 python-dateutil
 click>=8.0.0
-numpy
-unidecode
-setuptools>=51.0.0
-rich
-wheel
-colorama>=0.4
-black>=22.1.0
-pandas
-requests
 twine>=3.7.1
-build
+requests
+colorama>=0.4
+setuptools>=51.0.0
+numpy
+pipx
+matplotlib
 
 [autoimport]
 autoimport
 
 [beautiful]
 rich
 
@@ -49,39 +49,39 @@
 [click]
 click>=8.0.0
 
 [colorama]
 colorama>=0.4
 
 [dev]
-virtualenv>=20.13.0
-rich
-sphinx_rtd_theme
-sphinx
-wheel
-click>=8.0.0
 colorama>=0.4
-pipx
 pytest>=6.2.5
-unidecode
-twine>=3.7.1
 build
 setuptools>=51.0.0
+sphinx
+click>=8.0.0
+twine>=3.7.1
+sphinx_rtd_theme
+wheel
+rich
+pipx
+unidecode
+virtualenv>=20.13.0
 
 [extra]
-matplotlib
-scipy
-python-dateutil
-click>=8.0.0
 colorama>=0.4
-LunarCalendar>=0.0.9
+python-dateutil
 numpy
+click>=8.0.0
 pandas
-requests
+scipy
+LunarCalendar>=0.0.9
 unidecode
+requests
+matplotlib
 
 [fixers]
 autoimport
 black>=22.1.0
 
 [matplotlib]
 matplotlib
```

### Comparing `absfuyu-2.1.1/tests/test_DictKai.py` & `absfuyu-2.2.0/tests/test_DictKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_Generator.py` & `absfuyu-2.2.0/tests/test_Generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_IntNumber.py` & `absfuyu-2.2.0/tests/test_IntNumber.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_ListKai.py` & `absfuyu-2.2.0/tests/test_ListKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_Text.py` & `absfuyu-2.2.0/tests/test_Text.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_api.py` & `absfuyu-2.2.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_config.py` & `absfuyu-2.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_converter.py` & `absfuyu-2.2.0/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_obfuscator.py` & `absfuyu-2.2.0/tests/test_obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_path.py` & `absfuyu-2.2.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.1/tests/test_util.py` & `absfuyu-2.2.0/tests/test_util.py`

 * *Files identical despite different names*

