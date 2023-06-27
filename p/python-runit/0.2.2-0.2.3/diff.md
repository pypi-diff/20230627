# Comparing `tmp/python-runit-0.2.2.tar.gz` & `tmp/python-runit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-runit-0.2.2.tar", last modified: Thu Jun 22 17:28:49 2023, max compression
+gzip compressed data, was "python-runit-0.2.3.tar", last modified: Tue Jun 27 15:33:30 2023, max compression
```

## Comparing `python-runit-0.2.2.tar` & `python-runit-0.2.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.961460 python-runit-0.2.2/
--rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4703 2023-06-22 17:28:49.959507 python-runit-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:48.880047 python-runit-0.2.2/python_runit.egg-info/
--rw-rw-rw-   0        0        0     4703 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1528 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-22 17:28:48.000000 python-runit-0.2.2/python_runit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:48.982051 python-runit-0.2.2/runit/
--rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/Request.py
--rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.2.2/runit/__init__.py
--rw-rw-rw-   0        0        0    13015 2023-06-22 17:24:28.000000 python-runit-0.2.2/runit/cli.py
--rw-rw-rw-   0        0        0     2037 2023-06-22 17:25:15.000000 python-runit-0.2.2/runit/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.041050 python-runit-0.2.2/runit/languages/
--rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/languages/__init__.py
--rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/languages/javascript.py
--rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/languages/multi.py
--rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/languages/php.py
--rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/languages/python.py
--rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/languages/runtime.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.060052 python-runit-0.2.2/runit/modules/
--rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/modules/__init__.py
--rw-rw-rw-   0        0        0     8941 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/modules/account.py
--rw-rw-rw-   0        0        0    13030 2023-06-19 19:13:55.000000 python-runit-0.2.2/runit/runit.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.254048 python-runit-0.2.2/runit/templates/
--rw-rw-rw-   0        0        0       67 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/.runitignore
--rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/404.html
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.344827 python-runit-0.2.2/runit/templates/javascript/
--rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.2.2/runit/templates/javascript/.env
--rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/javascript/main.js
--rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/javascript/package.json
--rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/javascript/runit.json
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.540388 python-runit-0.2.2/runit/templates/multi/
--rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/application.py
--rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/composer.json
--rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/index.php
--rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/main.js
--rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/package.json
--rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/request.php
--rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/requirements.txt
--rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/multi/test.php
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.578665 python-runit-0.2.2/runit/templates/php/
--rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.2.2/runit/templates/php/.env
--rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/php/composer.json
--rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/php/index.php
--rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/php/runit.json
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.659243 python-runit-0.2.2/runit/templates/python/
--rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.2.2/runit/templates/python/.env
--rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/python/application.py
--rw-rw-rw-   0        0        0      363 2023-06-19 19:13:55.000000 python-runit-0.2.2/runit/templates/python/requirements.txt
--rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/python/runit.json
--rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/templates/request.php
--rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/templates/runit.json
--rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:48.821245 python-runit-0.2.2/runit/tools/
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.814464 python-runit-0.2.2/runit/tools/javascript/
--rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.2.2/runit/tools/javascript/loader.js
--rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.2.2/runit/tools/javascript/runner.js
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.947460 python-runit-0.2.2/runit/tools/php/
--rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/php/loader.php
--rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/php/runner.php
-drwxrwxrwx   0        0        0        0 2023-06-22 17:28:49.955462 python-runit-0.2.2/runit/tools/python/
--rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/python/loader.py
--rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.2.2/runit/tools/python/runner.py
--rw-rw-rw-   0        0        0       42 2023-06-22 17:28:49.962465 python-runit-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-06-22 17:25:23.000000 python-runit-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:30.533163 python-runit-0.2.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4703 2023-06-27 15:33:30.531160 python-runit-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:28.952931 python-runit-0.2.3/python_runit.egg-info/
+-rw-rw-rw-   0        0        0     4703 2023-06-27 15:33:28.000000 python-runit-0.2.3/python_runit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1528 2023-06-27 15:33:28.000000 python-runit-0.2.3/python_runit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:33:28.000000 python-runit-0.2.3/python_runit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-27 15:33:28.000000 python-runit-0.2.3/python_runit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2023-06-27 15:33:28.000000 python-runit-0.2.3/python_runit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 15:33:28.000000 python-runit-0.2.3/python_runit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:29.224683 python-runit-0.2.3/runit/
+-rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/Request.py
+-rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.2.3/runit/__init__.py
+-rw-rw-rw-   0        0        0    13479 2023-06-27 15:13:04.000000 python-runit-0.2.3/runit/cli.py
+-rw-rw-rw-   0        0        0     2037 2023-06-27 15:22:47.000000 python-runit-0.2.3/runit/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:29.312418 python-runit-0.2.3/runit/languages/
+-rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/languages/__init__.py
+-rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/languages/javascript.py
+-rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/languages/multi.py
+-rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/languages/php.py
+-rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/languages/python.py
+-rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/languages/runtime.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:29.334420 python-runit-0.2.3/runit/modules/
+-rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/modules/__init__.py
+-rw-rw-rw-   0        0        0     9017 2023-06-27 14:49:27.000000 python-runit-0.2.3/runit/modules/account.py
+-rw-rw-rw-   0        0        0    13372 2023-06-27 15:14:41.000000 python-runit-0.2.3/runit/runit.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:29.727064 python-runit-0.2.3/runit/templates/
+-rw-rw-rw-   0        0        0       82 2023-06-27 14:03:34.000000 python-runit-0.2.3/runit/templates/.runitignore
+-rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/templates/404.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:29.805054 python-runit-0.2.3/runit/templates/javascript/
+-rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.2.3/runit/templates/javascript/.env
+-rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/templates/javascript/main.js
+-rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/templates/javascript/package.json
+-rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/javascript/runit.json
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:29.879058 python-runit-0.2.3/runit/templates/multi/
+-rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/application.py
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/composer.json
+-rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/index.php
+-rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/main.js
+-rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/package.json
+-rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/request.php
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/requirements.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/multi/test.php
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:30.199354 python-runit-0.2.3/runit/templates/php/
+-rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.2.3/runit/templates/php/.env
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/php/composer.json
+-rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/templates/php/index.php
+-rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/php/runit.json
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:30.249950 python-runit-0.2.3/runit/templates/python/
+-rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.2.3/runit/templates/python/.env
+-rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/templates/python/application.py
+-rw-rw-rw-   0        0        0      363 2023-06-19 19:13:55.000000 python-runit-0.2.3/runit/templates/python/requirements.txt
+-rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/python/runit.json
+-rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/templates/request.php
+-rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/templates/runit.json
+-rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/test.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:28.641192 python-runit-0.2.3/runit/tools/
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:30.449164 python-runit-0.2.3/runit/tools/javascript/
+-rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.2.3/runit/tools/javascript/loader.js
+-rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.2.3/runit/tools/javascript/runner.js
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:30.503158 python-runit-0.2.3/runit/tools/php/
+-rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/tools/php/loader.php
+-rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/tools/php/runner.php
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:30.525162 python-runit-0.2.3/runit/tools/python/
+-rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/tools/python/loader.py
+-rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.2.3/runit/tools/python/runner.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:33:30.534162 python-runit-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-06-27 15:22:38.000000 python-runit-0.2.3/setup.py
```

### Comparing `python-runit-0.2.2/LICENSE` & `python-runit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/PKG-INFO` & `python-runit-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-runit-0.2.2/README.md` & `python-runit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/python_runit.egg-info/PKG-INFO` & `python-runit-0.2.3/python_runit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-runit-0.2.2/python_runit.egg-info/SOURCES.txt` & `python-runit-0.2.3/python_runit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/Request.py` & `python-runit-0.2.3/runit/Request.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/cli.py` & `python-runit-0.2.3/runit/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 import shelve
 import getpass
 import argparse
 from typing import Type, Optional
+from threading import Thread
 
 from fastapi import FastAPI, Request
 from dotenv import load_dotenv, set_key, find_dotenv, dotenv_values
 
 from .languages import LanguageParser
 from .modules import Account
 from .runit import RunIt
@@ -99,22 +100,34 @@
 
             if args.shell:
                 print(project.serve(args.function, args.arguments, args.file))
             else:
                 StartWebserver(project, args.host, args.port)
 
 def clone(args):
+    CURDIR = os.path.realpath(os.curdir)
     Account.isauthenticated({})
     user = Account.user()
     
-    project_path = os.path.join(os.path.basename(os.path.join(os.path.realpath(__file__), args.project_name)))
+    project_path = os.path.join(CURDIR, args.project_name)
     if not os.path.exists(project_path):
         os.mkdir(project_path)
+
+    print(f'[+] Cloning project into {args.project_name}...')
+    downloaded_file = Account.clone_project(args.project_name)
+
+    filepath = os.path.join(project_path, f"{args.project_name}.zip")
+    with open(filepath, 'wb') as zip_file:
+        zip_file.write(downloaded_file)
+    print('[!] Cloning complete')
+    RunIt.extract_project(filepath)
     os.chdir(project_path)
-    Account.clone_project(args.project_name)
+    runit = RunIt(**RunIt.load_config())
+    print(runit)
+    Thread(target=runit.install_dependency_packages, args=()).start()
         
 def publish(args):
     global CONFIG_FILE
     CONFIG_FILE = args.config
 
     global BASE_HEADERS
     # token = load_token()
```

### Comparing `python-runit-0.2.2/runit/constants.py` & `python-runit-0.2.3/runit/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = os.path.realpath(os.curdir)
```

### Comparing `python-runit-0.2.2/runit/languages/__init__.py` & `python-runit-0.2.3/runit/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/languages/multi.py` & `python-runit-0.2.3/runit/languages/multi.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/languages/runtime.py` & `python-runit-0.2.3/runit/languages/runtime.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/modules/account.py` & `python-runit-0.2.3/runit/modules/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,21 +233,22 @@
             global BASE_HEADERS
             token = load_token()
 
             BASE_HEADERS['Authorization'] = f"Bearer {token}"
             
             url = BASE_API + f'projects/clone/{project}/'
 
-            req = requests.get(url, headers=BASE_HEADERS)
-            print(req.headers)
-            result = req.json()
+            response = requests.get(url, headers=BASE_HEADERS)
 
-            if 'msg' in result.keys() and len(result['msg']):
-                raise Exception(f"[Error] {result['msg']}")
-            return result
+            if (response.headers['Content-Type'] == 'application/json'):
+                result = response.json()
+
+                if 'msg' in result.keys() and len(result['msg']):
+                    raise Exception(f"[Error] {result['msg']}")
+            return response.content
 
         except Exception as e:
             print(str(e))
             sys.exit(1)
     
     @staticmethod
     def create_project(args):
```

### Comparing `python-runit-0.2.2/runit/runit.py` & `python-runit-0.2.3/runit/runit.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 import sys
 import json
 from zipfile import ZipFile
 from io import TextIOWrapper
 from typing import Optional, Union
+from threading import Thread
 
 from flask import request
 from dotenv import load_dotenv
 
 from .languages import LanguageParser
 from .constants import TEMPLATES_FOLDER, STARTER_FILES, NOT_FOUND_FILE, \
         CONFIG_FILE, STARTER_CONFIG_FILE, IS_RUNNING, PROJECTS_DIR, \
@@ -34,15 +35,16 @@
         self.start_file = start_file if start_file else STARTER_FILES[self.language]
         self.create_config()
         
         if not RunIt.has_config_file() and not is_file:
             self.create_folder()
             self.dump_config()
             self.create_starter_files()
-            self.language_depending_packaging()
+            packages_install_thread = Thread(target=self.install_dependency_packages, args=())
+            packages_install_thread.start()
     
     def __repr__(self):
         return json.dumps(self.config, indent=4)
 
     @staticmethod
     def exists(name):
         return os.path.exists(os.path.join(os.curdir, name))
@@ -218,26 +220,28 @@
         self.config['private'] = self.private
         self.config['start_file'] = self.start_file
         self.config['author'] = self.author
         json.dump(self.config, config_file, indent=4)
         config_file.close()
     
     def compress(self):
-        os.chdir(CURRENT_PROJECT_DIR)
-
+        # os.chdir(CURRENT_PROJECT_DIR)
         zipname = f'{self.name}.zip'
         
-        exclude_list = [zipname, 'account.db']
+        exclude_list = [zipname, 'account.db', '.git', '.venv', 'venv']
         
-        with open('.runitignore', 'rt') as file:
-            for line in file.readlines():
-                if line:
-                    exclude_list.append(os.path.normpath(line.strip()))
+        if '.runitignore' in os.listdir():
+            with open('.runitignore', 'rt') as file:
+                for line in file.readlines():
+                    if line:
+                        exclude_list.append(os.path.normpath(line.strip()))
         
-        del exclude_list[exclude_list.index('.')]
+        if '.' in exclude_list:
+            del exclude_list[exclude_list.index('.')]
+
         with ZipFile(zipname, 'w') as zipobj:
             print('[!] Compressing Project Files...')
             for folderName, subfolders, filenames in os.walk(os.curdir):
                 
                 for filename in filenames:
                     if not os.path.normpath(os.path.dirname(folderName)).split(os.path.sep)[0] in exclude_list:
                         filepath = os.path.join(folderName,  filename)
@@ -278,15 +282,15 @@
             with open(os.path.join(os.curdir, self.name, NOT_FOUND_FILE), 'wt') as error:
                 error.write(file.read())
         
         with open(os.path.join(TEMPLATES_FOLDER, DOT_RUNIT_IGNORE),'rt') as file:
             with open(os.path.join(os.curdir, self.name, DOT_RUNIT_IGNORE), 'wt') as dotrunitignore:
                 dotrunitignore.write(file.read())
     
-    def language_depending_packaging(self):
+    def install_dependency_packages(self):
         # os.chdir(os.path.join(os.curdir, self.name))
         packaging_functions = {}
         packaging_functions['javascript'] = self.update_and_install_package_json
         packaging_functions['php'] = self.update_and_install_composer_json
         packaging_functions['python'] = self.install_python_packages
         packaging_functions['multi'] = self.install_all_language_packages
         packaging_functions[self.language]()
@@ -327,29 +331,31 @@
         package_file = open('composer.json', 'rt')
         package_details = json.load(package_file)
         package_file.close()
         
         package_details['name'] = f"runit/{self.name.replace('-', '_')}"
         package_details['author'] = self.author
         
-        package_file = open('composer.json', 'wt')
-        json.dump(package_details, package_file, indent=4)
-        package_file.close()
+        with open('composer.json', 'wt') as package_file:
+            json.dump(package_details, package_file, indent=4)
+
         # try:
         #     print('[-] Installing php packages...')
         #     os.system('composer install')
         # except Exception as e:
         #     print(str(e))
         #     print("[!] Couldn't install packages")
         #     print("[~] Try again manually later.")
     
     def install_python_packages(self):
         print("[-] Creating virtual environment")
         os.system(f"python -m venv venv")
         pip_path = os.path.join(os.curdir, 'venv', 'Scripts', 'pip.exe')
+        if sys.platform != 'win32':
+            pip_path = f".\{os.path.join(os.curdir, 'venv', 'bin', 'pip')}"
         try:
             print("[-] Installing python packages")
             activate_install_instructions = f"""
             {pip_path} install -r requirements.txt
             """.strip()
             os.system(activate_install_instructions)
         except Exception as e:
```

### Comparing `python-runit-0.2.2/runit/templates/404.html` & `python-runit-0.2.3/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/templates/multi/application.py` & `python-runit-0.2.3/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/templates/python/application.py` & `python-runit-0.2.3/runit/templates/python/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/tools/php/runner.php` & `python-runit-0.2.3/runit/tools/php/runner.php`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/runit/tools/python/runner.py` & `python-runit-0.2.3/runit/tools/python/runner.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.2.2/setup.py` & `python-runit-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='python-runit',
     version=VERSION,
```

