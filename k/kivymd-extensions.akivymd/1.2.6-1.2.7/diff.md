# Comparing `tmp/kivymd_extensions.akivymd-1.2.6.tar.gz` & `tmp/kivymd_extensions.akivymd-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kivymd_extensions.akivymd-1.2.6.tar", last modified: Sun Apr 25 19:08:06 2021, max compression
+gzip compressed data, was "dist/kivymd_extensions.akivymd-1.2.7.tar", last modified: Mon Jun 26 22:41:58 2023, max compression
```

## Comparing `kivymd_extensions.akivymd-1.2.6.tar` & `kivymd_extensions.akivymd-1.2.7.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4579 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/factory_registers.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/badgelayout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/behaviors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/behaviors/addwidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/behaviors/labelanimation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/bottomappbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5978 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/bottomnavigation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6112 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/bottomnavigation2.py
--rw-r--r--   0 runner    (1001) docker     (121)    15526 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/charts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6073 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/datepicker.py
--rw-r--r--   0 runner    (1001) docker     (121)     8619 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7143 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/hintwidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     4756 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/imageview.py
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     8758 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/navigationrail.py
--rw-r--r--   0 runner    (1001) docker     (121)     6333 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (121)     6255 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/progressbutton.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/progresswidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     5576 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/selectionlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     4820 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/silverappbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    13172 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/spinners.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/statusbarcolor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8515 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/swipemenu.py
--rw-r--r--   0 runner    (1001) docker     (121)    11409 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    12262 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/utils/draw_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4579 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      737 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-04-25 19:08:06.000000 kivymd_extensions.akivymd-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-04-25 19:08:01.000000 kivymd_extensions.akivymd-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/factory_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/badgelayout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/behaviors/addwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/behaviors/labelanimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/bottomappbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/bottomnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/bottomnavigation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/buttonpanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/cardstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/datepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/hintwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/navigationrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/progressbutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/progresswidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/selectionlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/silverappbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/spinners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/statusbarcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/swipemenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/utils/draw_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 22:41:58.000000 kivymd_extensions.akivymd-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-26 22:41:50.000000 kivymd_extensions.akivymd-1.2.7/setup.py
```

### Comparing `kivymd_extensions.akivymd-1.2.6/LICENSE` & `kivymd_extensions.akivymd-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/PKG-INFO` & `kivymd_extensions.akivymd-1.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,16 @@
 Metadata-Version: 2.1
 Name: kivymd_extensions.akivymd
-Version: 1.2.6
+Version: 1.2.7
 Summary: A set of fancy widgets for KivyMD
 Home-page: https://github.com/kivymd-extensions/akivymd
 Author: quitegreensky, KivyMD Team and other contributors
 Author-email: quitegreensky@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/kivymd-extensions/akivymd/issues
-Description: # Awesome KivyMD
-        
-        Awesome KivyMD is a package containing customized and non-material widgets for KivyMD.
-        
-        <p align="center">
-            <img align="center" width="512" src="https://raw.githubusercontent.com/quitegreensky/akivymd/master/images/preview.gif"/>
-        </p>
-        
-        ## Installation
-        
-        ```bash
-        pip install kivymd_extensions.akivymd
-        
-        #or 
-        
-        pip install https://github.com/kivymd-extensions/akivymd/archive/main.zip
-        ```
-        
-        ## Usage with Buildozer
-        
-        ```bash
-        requirements = https://github.com/kivymd-extensions/akivymd/archive/main.zip
-        ```
-        
-        ### Dependencies:
-        
-        - [KivyMD](https://github.com/kivymd/KivyMD) >= 0.104.2 (from master branch)
-        - [Kivy](https://github.com/kivy/kivy) >= 1.11.1 ([Installation](https://kivy.org/doc/stable/gettingstarted/installation.html))
-        - [Python 3.6+](https://www.python.org/)
-        
-        ## Documentation
-        
-        ### Usage
-        
-        ```python
-        from kivy.lang import Builder
-        
-        from kivymd.app import MDApp
-        import kivymd_extensions.akivymd
-        
-        KV = """
-        <NavigationButton@Button_Item>
-            icon_color: app.theme_cls.text_color
-            text_color: app.theme_cls.text_color
-            button_bg_color: app.theme_cls.primary_color
-            mode: 'color_on_active'
-            badge_disabled: True
-        
-        
-        MDScreen:
-        
-            AKBottomNavigation2:
-                bg_color: app.theme_cls.bg_darkest
-                
-                NavigationButton:
-                    text: 'Alert'
-                    icon: 'bell-outline'
-                
-                NavigationButton:
-                    text: 'Bank'
-                    icon: 'bank-outline'
-                
-                NavigationButton:
-                    text: 'Download'
-                    icon: 'arrow-down-bold-outline'
-        """
-        
-        
-        class Test(MDApp):
-            def build(self):
-                return Builder.load_string(KV)
-        
-        
-        Test().run()
-        ```
-        
-        ## Examples
-        
-        ```bash
-        git clone https://github.com/kivymd-extensions/akivymd.git
-        cd akivymd
-        cd examples/full_example
-        python main.py
-        ```
-        
-        ## Support
-        
-        If you need assistance or you have a question, you can ask for help on our mailing list:
-        
-        - **Discord server:** https://discord.gg/wu3qBST
-        - _Email:_ kivydevelopment@gmail.com
-        
-        ## License
-        
-        [MIT License](LICENSE)
-        
 Keywords: kivymd_extensions,kivymd,kivy,material,ui
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -127,11 +31,116 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
+
+# Awesome KivyMD
+
+Awesome KivyMD is a package containing customized and non-material widgets for KivyMD.
+
+<p align="center">
+    <img align="center" width="512" src="https://raw.githubusercontent.com/quitegreensky/akivymd/master/images/preview.gif"/>
+</p>
+
+## Installation
+
+```bash
+pip install kivymd_extensions.akivymd
+
+#or
+
+pip install https://github.com/kivymd-extensions/akivymd/archive/main.zip
+```
+
+## Usage with Buildozer
+
+```bash
+requirements = https://github.com/kivymd-extensions/akivymd/archive/main.zip
+```
+
+### Dependencies:
+
+- [KivyMD](https://github.com/kivymd/KivyMD) >= 0.104.2 (from master branch)
+- [Kivy](https://github.com/kivy/kivy) >= 1.11.1 ([Installation](https://kivy.org/doc/stable/gettingstarted/installation.html))
+- [Python 3.6+](https://www.python.org/)
+
+## Documentation
+
+### Usage
+
+```python
+from kivy.lang import Builder
+
+from kivymd.app import MDApp
+import kivymd_extensions.akivymd
+
+KV = """
+<NavigationButton@Button_Item>
+    icon_color: app.theme_cls.text_color
+    text_color: app.theme_cls.text_color
+    button_bg_color: app.theme_cls.primary_color
+    mode: 'color_on_active'
+    badge_disabled: True
+
+
+MDScreen:
+
+    AKBottomNavigation2:
+        bg_color: app.theme_cls.bg_darkest
+
+        NavigationButton:
+            text: 'Alert'
+            icon: 'bell-outline'
+
+        NavigationButton:
+            text: 'Bank'
+            icon: 'bank-outline'
+
+        NavigationButton:
+            text: 'Download'
+            icon: 'arrow-down-bold-outline'
+"""
+
+
+class Test(MDApp):
+    def build(self):
+        return Builder.load_string(KV)
+
+
+Test().run()
+```
+
+## Examples
+
+```bash
+git clone https://github.com/kivymd-extensions/akivymd.git
+cd akivymd
+cd examples/full_example
+python main.py
+```
+
+## Build Docs
+
+```bash
+git clone https://github.com/kivymd-extensions/akivymd.git
+cd docs
+sphinx-build -b html sources ./_build
+```
+
+## Support
+
+If you need assistance or you have a question, you can ask for help on our mailing list:
+
+- **Discord server:** https://discord.gg/wu3qBST
+- _Email:_ kivydevelopment@gmail.com
+
+## License
+
+[MIT License](LICENSE)
```

### Comparing `kivymd_extensions.akivymd-1.2.6/README.md` & `kivymd_extensions.akivymd-1.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 </p>
 
 ## Installation
 
 ```bash
 pip install kivymd_extensions.akivymd
 
-#or 
+#or
 
 pip install https://github.com/kivymd-extensions/akivymd/archive/main.zip
 ```
 
 ## Usage with Buildozer
 
 ```bash
@@ -47,23 +47,23 @@
     badge_disabled: True
 
 
 MDScreen:
 
     AKBottomNavigation2:
         bg_color: app.theme_cls.bg_darkest
-        
+
         NavigationButton:
             text: 'Alert'
             icon: 'bell-outline'
-        
+
         NavigationButton:
             text: 'Bank'
             icon: 'bank-outline'
-        
+
         NavigationButton:
             text: 'Download'
             icon: 'arrow-down-bold-outline'
 """
 
 
 class Test(MDApp):
@@ -79,14 +79,22 @@
 ```bash
 git clone https://github.com/kivymd-extensions/akivymd.git
 cd akivymd
 cd examples/full_example
 python main.py
 ```
 
+## Build Docs
+
+```bash
+git clone https://github.com/kivymd-extensions/akivymd.git
+cd docs
+sphinx-build -b html sources ./_build
+```
+
 ## Support
 
 If you need assistance or you have a question, you can ask for help on our mailing list:
 
 - **Discord server:** https://discord.gg/wu3qBST
 - _Email:_ kivydevelopment@gmail.com
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/factory_registers.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/factory_registers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 r("AKBadgeLayout", module=f"{a}.uix.badgelayout")
 r("AKFloatingRoundedAppbar", module=f"{a}.uix.bottomappbar")
 r("AKFloatingRoundedAppbarAvatarItem", module=f"{a}.uix.bottomappbar")
 r("AKFloatingRoundedAppbarButtonItem", module=f"{a}.uix.bottomappbar")
 r("AKBottomNavigation", module=f"{a}.uix.bottomnavigation")
 r("AKBottomNavigation2", module=f"{a}.uix.bottomnavigation2")
 r("Button_Item", module=f"{a}.uix.bottomnavigation2")
+r("AKButtonPanel", module=f"{a}.uix.buttonpanel")
+r("AKCardStack", module=f"{a}.uix.cardstack")
 r("AKImageLoader", module=f"{a}.uix.loaders")
 r("AKLabelLoader", module=f"{a}.uix.loaders")
 r("AKImageViewer", module=f"{a}.uix.imageview")
 r("AKImageViewerItem", module=f"{a}.uix.imageview")
 r("AKOnboarding", module=f"{a}.uix.onboarding")
 r("AKOnboardingItem", module=f"{a}.uix.onboarding")
 r("AKPieChart", module=f"{a}.uix.charts")
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/behaviors/addwidget.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/behaviors/addwidget.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/behaviors/labelanimation.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/behaviors/labelanimation.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/bottomnavigation.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/onboarding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,198 +1,203 @@
 from kivy.animation import Animation
 from kivy.clock import Clock
 from kivy.core.window import Window
-from kivy.lang.builder import Builder
+from kivy.event import EventDispatcher
+from kivy.lang import Builder
 from kivy.metrics import dp
-from kivy.properties import ListProperty, NumericProperty, StringProperty
+from kivy.properties import (
+    BooleanProperty,
+    ListProperty,
+    NumericProperty,
+    StringProperty,
+)
 from kivy.uix.boxlayout import BoxLayout
+from kivy.uix.carousel import Carousel
+from kivy.uix.widget import Widget
 from kivymd.theming import ThemableBehavior
-from kivymd.uix.button import MDIconButton
-from kivymd.uix.label import MDLabel
-
-__all__ = ("AKBottomNavigation",)
 
 Builder.load_string(
     """
-<_AKLabel>
-    size_hint: None, None
-    size: dp(48), dp(48)
-    font_style: "Caption"
-    halign: "center"
-    valign: "center"
-    theme_text_color: "Custom"
-    text_color: root.text_color if root.text_color else root.theme_cls.primary_light
-
-
-<_AKButton>
-    theme_text_color: "Custom"
-    text_color: root.icon_color if root.icon_color else root.theme_cls.primary_color
+<ItemCircles>:
+    size_hint_x: None
+    canvas.before:
+        Color:
+            rgba: root._circles_color
+        Line:
+            circle: [self.pos[0] + self.width / 2, self.pos[1] + self.height / 2, self.width / 2]
+            width: dp(1)
+
 
+<AKOnboardingItem>:
 
-<AKBottomNavigation>:
+
+<AKOnboarding>:
     orientation: "vertical"
-    size_hint_y: None
-    height: self.minimum_height
-    BoxLayout:
-        size_hint_y: None
-        height: dp(14)
 
-        canvas.before:
-            Color:
-                rgba: root.bar_color if root.bar_color else root.theme_cls.primary_color
-            Rectangle:
-                pos: self.pos
-                size: self.size
+    MyCarousel:
+        min_move:root.min_move
+        anim_type: root.anim_type
+        anim_move_duration: root.anim_move_duration
+        id: carousel
 
-    BoxLayout:
+    FloatLayout:
+        id: rounded_box
         size_hint_y: None
-        height: dp(56)
-
+        height: circles_box.y + circles_box.height * 2
         canvas.before:
             Color:
-                rgba: root.bg_color if root.bg_color else root.theme_cls.bg_dark
-            Rectangle:
+                rgba: root.bottom_bar_color if root.bottom_bar_color else app.theme_cls.bg_dark
+                a: 1 if root.show_bottom_bar else 0
+            RoundedRectangle:
                 pos: self.pos
                 size: self.size
+                radius: root.bottom_bar_radius
 
         Widget:
-            id: _bubble
-            bubble_x: 0
+            id: ghost_circle
             size_hint: None, None
-            size: root.width, dp(70)
             canvas.before:
                 Color:
-                    rgba: root.bar_color if root.bar_color else root.theme_cls.primary_color
-                Rectangle:
-                    pos: self.bubble_x, dp(28)
-                    size: dp(112), dp(28)
+                    rgba: root.circles_color if root.circles_color else root.theme_cls.primary_color
                 Ellipse:
-                    pos: self.bubble_x + dp(28), 0
-                    size: dp(56), dp(56)
-                Color:
-                    rgba: root.bg_color if root.bg_color else root.theme_cls.bg_dark
-                Ellipse:
-                    pos: self.bubble_x- dp(28), 0
-                    size: dp(56), dp(56)
-                Ellipse:
-                    pos: self.bubble_x + dp(84), 0
-                    size: dp(56), dp(56)
+                    pos: self.pos
+                    size: self.size
 
-            FloatLayout:
-                id: _text_bar
-                size_hint: None, None
-                size: root.width, dp(56)
-
-            FloatLayout:
-                id: _buttons_bar
-                size_hint: None, None
-                size: root.width, dp(70)
+        BoxLayout:
+            id: circles_box
+            pos: rounded_box.width / 2 - self.width / 2, rounded_box.height / 2 - self.height / 2
+            size_hint: None,None
+            size: self.minimum_width, root.circles_size
+            spacing: root.circles_size / 2
+
+        MDFlatButton:
+            text: "Skip"
+            on_release: root._on_finish_dispatch()
+            disabled: False if root.skip_button else True
+            opacity: 1 if root.skip_button else 0
+            theme_text_color: "Custom"
+            text_color: root.circles_color if root.circles_color else root.theme_cls.primary_color
+            pos_hint: {"right": .95, "center_y": .5}
 """
 )
 
 
-class _AKLabel(MDLabel):
-    text_color = ListProperty()
+class ItemCircles(ThemableBehavior, Widget):
+    _circles_color = ListProperty(None)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
-class _AKButton(MDIconButton):
-    icon_color = ListProperty()
-
+class MyCarousel(ThemableBehavior, Carousel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        Clock.schedule_once(lambda x: self._update())
+        Clock.schedule_once(lambda x: self._add_circles())
+        Window.bind(on_resize=self._on_resize)
 
-    def on_release(self):
-        self.root.set_current(self.parent.children.index(self))
+    def _add_circles(self):
+        self.total_circles = len(self.slides) - 1
 
-    def _update(self):
-        self.root = self.parent.parent.parent.parent
+        if self.parent.circles_color:
+            circle_color = self.parent.circles_color
+        else:
+            circle_color = self.theme_cls.primary_color
+
+        for _ in range(self.total_circles + 1):
+            self.parent.ids.circles_box.add_widget(
+                ItemCircles(
+                    width=self.parent.circles_size, _circles_color=circle_color
+                )
+            )
 
+        self._current_circle = self.total_circles
+        Clock.schedule_once(lambda x: self._set_current_circle(animation=False))
+
+    def on_size(self, *args):
+        Clock.schedule_once(lambda x: self._set_current_circle(animation=False))
+        return super().on_size(*args)
+
+    def reset(self):
+        self._current_circle = self.total_circles
+        self._set_current_circle()
+        self.load_slide(self.slides[0])
+
+    def _set_current_circle(self, mode=None, animation=True):
+        if mode == "next":
+            if self._current_circle > 0:
+                self._current_circle -= 1
+            else:
+                self.parent._on_finish_dispatch()
+
+        elif mode == "previous":
+            if self._current_circle < self.total_circles:
+                self._current_circle += 1
+        if animation:
+            anim = Animation(
+                pos=self.parent.ids.circles_box.children[
+                    self._current_circle
+                ].pos,
+                t=self.anim_type,
+                duration=self.anim_move_duration,
+            )
+            anim.start(self.parent.ids.ghost_circle)
+        else:
+            self.parent.ids.ghost_circle.pos = (
+                self.parent.ids.circles_box.children[self._current_circle].pos
+            )
+
+    def on_touch_up(self, touch):
+        if abs(self._offset) > self.width * self.min_move:
+
+            if self._offset > 0:  # previous screen
+                self._set_current_circle("previous")
+
+            elif self._offset < 0:  # next screen
+                self._set_current_circle("next")
+
+        return super().on_touch_up(touch)
+
+    def _on_resize(self, *args):
+        Clock.schedule_once(lambda x: self._set_current_circle(animation=False))
+
+
+class AKOnboardingItem(BoxLayout):
+    pass
 
-class AKBottomNavigation(ThemableBehavior, BoxLayout):
-    items = ListProperty()
-    bar_color = ListProperty()
-    icon_color = ListProperty()
-    text_color = ListProperty()
-    bg_color = ListProperty()
-    transition = StringProperty("out_sine")
-    duration = NumericProperty(0.2)
 
-    _selected = -1
+class AKOnboarding(ThemableBehavior, BoxLayout, EventDispatcher):
+
+    circles_size = NumericProperty(dp(20))
+    skip_button = BooleanProperty(True)
+    min_move = NumericProperty(0.05)
+    anim_type = StringProperty("out_quad")
+    anim_move_duration = NumericProperty(0.2)
+    bottom_bar_radius = ListProperty([dp(20), dp(20), 0, 0])
+    show_bottom_bar = BooleanProperty(True)
+    bottom_bar_color = ListProperty(None)
+    circles_color = ListProperty(None)
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        Window.bind(on_resize=self._on_resize)
+        super(AKOnboarding, self).__init__(**kwargs)
+        self.register_event_type("on_finish")
+        Clock.schedule_once(lambda x: self._update())
 
-    def _clear_bar(self):
-        self.ids._buttons_bar.clear_widgets()
-        self.ids._text_bar.clear_widgets()
-
-    def _update_items(self, items):
-        count = len(self.items)
-        section_x = 1 / (count + 1)
-        but_pos = section_x
-        for x in range(0, count):
-            button = _AKButton(
-                icon=self.items[x]["icon"],
-                pos_hint={"center_x": but_pos},
-                icon_color=self.icon_color,
-            )
-            button.bind(on_release=self.items[x]["on_release"])
+    def add_widget(self, widget, index=0, canvas=None):
+        if issubclass(widget.__class__, AKOnboardingItem):
+            self.ids.carousel.add_widget(widget)
+        else:
+            super().add_widget(widget, index=index, canvas=canvas)
+
+    def _on_finish_dispatch(self):
+        self.dispatch("on_finish")
 
-            label = _AKLabel(
-                text=self.items[x]["text"],
-                pos_hint={"center_x": but_pos},
-                opacity=0,
-                text_color=self.text_color,
-            )
+    def on_finish(self, *args):
+        pass
+
+    def reset(self):
+        return self.ids.carousel.reset()
 
-            self.ids._text_bar.add_widget(label)
-            self.ids._buttons_bar.add_widget(button)
-            but_pos += section_x
-        self.ids._bubble.bubble_x = Window.size[
-            0
-        ] * self.ids._buttons_bar.children[self._selected].pos_hint[
-            "center_x"
-        ] - dp(
-            56
-        )
-        self.ids._buttons_bar.children[self._selected].opacity = 0
-        self.ids._text_bar.children[self._selected].opacity = 1
-
-    def _on_resize(self, instance, width, height):
-        self.ids._bubble.bubble_x = width * self.ids._buttons_bar.children[
-            self._selected
-        ].pos_hint["center_x"] - dp(56)
-
-    def on_items(self, *args):
-        self._clear_bar()
-        return self._update_items(self.items)
-
-    def set_current(self, index):
-        current_item_button = self.ids._buttons_bar.children[index]
-        current_item_text = self.ids._text_bar.children[index]
-        AKBottomNavigation._selected = index
-
-        for x in self.ids._buttons_bar.children:  # button
-            x.opacity = 1
-
-        for x in self.ids._text_bar.children:  # text
-            x.opacity = 0
-
-        bubble_pos = current_item_button.x - dp(31)
-        anim_bubble = Animation(
-            bubble_x=bubble_pos, t=self.transition, duration=self.duration
-        )
-        anim_text_opacity = Animation(
-            opacity=1, t=self.transition, duration=self.duration
-        )
-        anim_icon_opacity = Animation(
-            opacity=0, t=self.transition, duration=self.duration
-        )
-
-        anim_icon_opacity.start(current_item_button)
-        anim_text_opacity.start(current_item_text)
-        anim_bubble.start(self.ids._bubble)
+    def on_size(self, *args):
+        self.ids.carousel.size = self.size
+
+    def _update(self):
+        self.ids.ghost_circle.size = [self.circles_size, self.circles_size]
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/charts.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 from kivymd_extensions.akivymd.helper import point_on_circle
 from kivymd_extensions.akivymd.utils.draw_tools import DrawTools
 
 """issues
 color_mode
 """
 
+__all__ = (
+    "AKPieChart",
+    "AKLineChart",
+    "AKBarChart",
+)
+
 Builder.load_string(
     """
 <PieChartNumberLabel>
     size_hint: None, None
     size: dp(40), dp(30)
     text: "%s\\n%d%%" % (root.title, root.percent)
     font_size: dp(10)
@@ -232,21 +238,21 @@
     label_size = NumericProperty("15dp")
     bars_color = ColorProperty([1, 1, 1, 1])
     line_width = NumericProperty("2dp")
     lines_color = ColorProperty([1, 1, 1, 1])
     lines = BooleanProperty(True)
     trim = BooleanProperty(True)
     _loaded = NumericProperty(1)
-    _myinit = True
     _labels_y_box = ObjectProperty()
     _labels_x_box = ObjectProperty()
     _canvas = ObjectProperty()
 
     def __init__(self, **kw):
         super().__init__(**kw)
+        self._myinit = True
         self.bind(
             _loaded=lambda *args: self._update(anim=True),
         )
         Clock.schedule_once(self.update)
 
     def _get_normalized_cor(self, val, mode, f_update=1):
         x_values = self.x_values
@@ -284,14 +290,15 @@
         self._myinit = True
         if self.anim:
             self._loaded = 0
             anim = Animation(_loaded=1, t=self.t, d=self.d)
             anim.start(self)
         else:
             self._update()
+            self._update()
 
     def _update(self, anim=False, *args):
         x_values = self.x_values
         y_values = self.y_values
         x_labels = self.x_labels
         y_labels = self.y_labels
         canvas = self._canvas.canvas
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/datepicker.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/datepicker.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/dialogs.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/dialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ObjectProperty,
     OptionProperty,
     StringProperty,
 )
 from kivy.uix.boxlayout import BoxLayout
 from kivy.uix.modalview import ModalView
 from kivymd.app import MDApp
-from kivymd.uix.behaviors import RectangularElevationBehavior
+from kivymd.uix.behaviors import CommonElevationBehavior
 from kivymd.uix.dialog import BaseDialog
 
 Builder.load_string(
     """
 #:import md_icons kivymd.icon_definitions.md_icons
 
 
@@ -81,15 +81,15 @@
 
         BoxLayout:
             id: content
     """
 )
 
 
-class MainAlertBox(RectangularElevationBehavior, BoxLayout):
+class MainAlertBox(CommonElevationBehavior, BoxLayout):
     pass
 
 
 class AKAlertDialog(BaseDialog):
     dialog_radius = NumericProperty("10dp")
     bg_color = ListProperty()
     size_portrait = ListProperty(["250dp", "350dp"])
@@ -104,15 +104,15 @@
     header_color = ListProperty()
     header_h_pos = StringProperty("center")
     header_v_pos = StringProperty("center")
     header_font_size = NumericProperty("55dp")
     progress_interval = NumericProperty(None)
     progress_width = NumericProperty("2dp")
     progress_color = ListProperty()
-    elevation = NumericProperty(10)
+    elevation = NumericProperty(2)
     content_cls = ObjectProperty()
     opening_duration = NumericProperty(0.2)
     dismiss_duration = NumericProperty(0.2)
 
     _orientation = StringProperty()
     _progress_value = NumericProperty()
 
@@ -125,16 +125,16 @@
     def _update(self, *args):
         self._get_orientation()
         Window.bind(on_touch_down=self._window_touch_down)
         Window.bind(on_touch_up=self._window_touch_up)
         Window.bind(on_touch_move=self._window_touch_move)
 
     def _collide_point_with_modal(self, pos):
-        if self.attach_to:
-            raise NotImplementedError
+        # if self.attach_to:
+        #     raise NotImplementedError
         for widget in Window.children:
             if issubclass(widget.__class__, ModalView):
                 if widget.collide_point(pos[0], pos[1]):
                     return widget
         return False
 
     def _get_top_modal(self):
@@ -216,21 +216,24 @@
 
     def on_dismiss(self):
         self._dismiss_animation()
         return super().on_dismiss()
 
     def _opening_animation(self):
         self.opacity = 0
+        _elevation = self.elevation
+        self.elevation = 0
         anim = Animation(
             opacity=1, duration=self.opening_duration, t="out_quad"
-        )
+        ) + Animation(elevation=_elevation, duration=self.opening_duration/2, t="out_quad")
         anim.start(self)
 
     def _dismiss_animation(self):
-        anim = Animation(
+        anim = Animation(elevation=0, duration=self.opening_duration/2, t="out_quad") + \
+            Animation(
             opacity=0, duration=self.dismiss_duration, t="out_quad"
         )
         anim.start(self)
 
     def _start_progress(self):
         if not self.progress_interval:
             return
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/hintwidget.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/hintwidget.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/imageview.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/imageview.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         size: scatter.size
         source: root.source
 
 <AKImageViewer>:
     id: _mainbox
     size_hint: (0.9, 0.4) if root.theme_cls.device_orientation == "portrait" else (0.9, 0.7)
     carousel: carousel
+    elevation: 0
 
     FloatLayout:
         Navigation_button:
             id: _left_button
             pos_hint: {"x": 0 , "center_y": .5}
             icon: "chevron-left"
             on_release:
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/loaders.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/loaders.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/navigationrail.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/navigationrail.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from kivy.animation import Animation
 from kivy.clock import Clock
 from kivy.lang.builder import Builder
 from kivy.properties import (
     BooleanProperty,
     ListProperty,
     NumericProperty,
+    ObjectProperty,
     StringProperty,
 )
 from kivy.uix.behaviors import ButtonBehavior
 from kivy.uix.boxlayout import BoxLayout
 from kivymd.theming import ThemableBehavior
 
 Builder.load_string(
@@ -17,30 +18,33 @@
 
 
 <AKNavigationrailCustomItem>:
 
 
 <AKNavigationrailItem>:
     size_hint_y: None
-    height: root.parent.parent.item_height
+    height: root._root.item_height
+    spacing: dp(5)
+    padding: dp(5)
     MDIcon:
         icon: root.icon
         size_hint_x: None
         width: root.height
         theme_text_color: "Custom"
         text_color: root.active_icon_color if root.active else root.icon_color
-        halign: "center"
+        pos_hint: {"center_x": .5, "center_y": .5}
 
     MDLabel:
         opacity: root.item_text_opacity
         text: root.text
         theme_text_color: "Custom"
         text_color: root.active_text_color if root.active else root.text_color
         halign: "left"
         valign: "center"
+        font_name: root.font_name if root.font_name else self.font_name
 
 
 <AKNavigationrail>
 
     BoxLayout:
         orientation: "vertical"
         id: items_box
@@ -107,14 +111,16 @@
     icon = StringProperty()
     text = StringProperty()
     text_color = ListProperty([0, 0, 0, 0])
     icon_color = ListProperty([0, 0, 0, 0])
     active_text_color = ListProperty([0, 0, 0, 0])
     active_icon_color = ListProperty([0, 0, 0, 0])
     active = BooleanProperty(False)
+    font_name = StringProperty("")
+    _root = ObjectProperty()
 
     item_text_opacity = NumericProperty(1)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         Clock.schedule_once(lambda x: self._update())
 
@@ -129,17 +135,16 @@
         if self.active_icon_color == [0, 0, 0, 0]:
             self.active_icon_color = self.theme_cls.primary_color
 
         if self.icon_color == [0, 0, 0, 0]:
             self.icon_color = self.theme_cls.text_color
 
     def on_release(self):
-        self.root = self.parent.parent
-        index = self.root.ids.items_box.children.index(self)
-        self.root.set_current(index, item_index=False)
+        index = self._root.ids.items_box.children.index(self)
+        self._root.set_current(index, item_index=False)
         return super().on_release()
 
 
 class AKNavigationrailCustomItem(AKNavigationrailItemBase):
     pass
 
 
@@ -266,16 +271,16 @@
 
     def on_size(self, *args):
         self.refresh_items()
 
     def add_widget(self, widget, index=0, canvas=None):
         if issubclass(widget.__class__, AKNavigationrailItem):
             self.ids.items_box.add_widget(widget)
-            Clock.schedule_once(lambda x: self.set_current(-1, anim=False), 1)
-
+            widget._root = self
+            widget.bind(pos=lambda *args: self.set_current(-1, anim=False))
         elif issubclass(widget.__class__, AKNavigationrailCustomItem):
             self.ids.items_box.add_widget(widget)
 
         elif issubclass(widget.__class__, AKNavigationrailContent):
             self.ids.content.add_widget(widget)
         else:
             return super().add_widget(widget, index=index, canvas=canvas)
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/progressbutton.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/progressbutton.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/progresswidget.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/progresswidget.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/rating.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/rating.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 Components/Rating
 =================
 
-
 Example
 -------
 
 .. code-block:: python
 
     from kivy.lang.builder import Builder
 
     from kivymd.app import MDApp
+    import kivymd_extensions.akivymd  # NOQA
 
     KV = '''
-    Screen:
+    MDScreen:
+
         AKRating:
             direction : 'lr'
             pos_hint: {'center_x': .5, 'center_y': .5}
             on_rate: print(self.get_rate())
     '''
 
     class Main(MDApp):
 
         def build(self):
             return Builder.load_string(KV)
 
 
     Main().run()
+
 """
 
 from kivy.clock import Clock
 from kivy.lang.builder import Builder
 from kivy.metrics import dp
 from kivy.properties import (
     ListProperty,
@@ -58,92 +60,103 @@
         halign: "center"
         valign: "center"
 
 
 <AKRating>
     size_hint: None, None
     size: self.minimum_size
+
     """
 )
 
 
 class _RaitingItem(ThemableBehavior, ButtonBehavior, BoxLayout, MagicBehavior):
     icon = StringProperty()
     text_color = ListProperty()
     font_size = NumericProperty()
     item_spacing = NumericProperty()
 
 
 class AKRating(ThemableBehavior, BoxLayout):
     """
     :Events:
+
         :attr:`on_rate`
             Called when an icon is clicked.
     """
 
     count = NumericProperty(5)
-    """Number of items.
+    """
+    Number of items.
 
     :attr:`count` is an :class:`~kivy.properties.NumericProperty`
     and defaults to `5`.
     """
 
     direction = OptionProperty("lr", options=["lr", "rl"])
-    """Direction of item selection. Can be `lr` for left to right or `rl` for right to left.
+    """
+    Direction of item selection. Can be `lr` for left to right or `rl` for right to left.
 
     :attr:`direction` is an :class:`~kivy.properties.OptionProperty`
     and defaults to `lr`.
     """
 
     normal_icon = StringProperty("star-outline")
-    """Normal icon.
+    """
+    Normal icon.
 
     :attr:`normal_icon` is an :class:`~kivy.properties.StringProperty`
     and defaults to `star-outline`.
     """
 
     active_icon = StringProperty("star")
-    """Active icon.
+    """
+    Active icon.
 
     :attr:`normal_icon` is an :class:`~kivy.properties.StringProperty`
     and defaults to `star`.
     """
 
     normal_color = ListProperty()
-    """Normal icon color.
+    """
+    Normal icon color.
 
     :attr:`normal_color` is an :class:`~kivy.properties.ListProperty`
     and defaults to primary color.
     """
 
     active_color = ListProperty()
-    """Active icon color.
+    """
+    Active icon color.
 
     :attr:`active_color` is an :class:`~kivy.properties.ListProperty`
     and defaults to accent color.
     """
 
     icon_size = NumericProperty(dp(30))
-    """The size of icons.
+    """
+    The size of icons.
 
     :attr:`icon_size` is an :class:`~kivy.properties.NumericProperty`
     and defaults to `dp(30)`.
     """
 
     item_spacing = NumericProperty(dp(7))
-    """The space between icons.
+    """
+    The space between icons.
 
     :attr:`item_spacing` is an :class:`~kivy.properties.NumericProperty`
     and defaults to `dp(7)`.
     """
 
     animation_type = OptionProperty(
         "twist", options=[False, "twist", "wobble", "shake", "grow"]
     )
-    """The animation type when an icon is clicked. The animations will be applied on active icons only.
+    """
+    The animation type when an icon is clicked. The animations will be applied on active icons only.
         Set to `False` for no animation.
 
     :attr:`animation_type` is an :class:`~kivy.properties.OptionProperty`
     and defaults to `twist`.
     """
 
     _selected = 0
@@ -209,11 +222,13 @@
     def _get_item_index(self, item):
         return self._get_children().index(item)
 
     def on_rate(self, *args):
         pass
 
     def set_rate(self, rate):
-        """Set current rate. """
+        """
+        Set current rate.
+        """
 
         self._selected = rate - 1
         self._update_items()
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/selectionlist.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/selectionlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,22 @@
     padding: dp(5)
     spacing: dp(5)
     on_release: root._choose_selection(_first_label.text)
 
     FloatLayout:
         Image:
             pos_hint: {"center_x": .5, "center_y": .5}
-            keep_ratio: True
+            fit_mode: "contain"
             source: root.source
 
         MDIcon:
             id: _box
             pos_hint: {"center_x": 0.9, "center_y": 0.9}
-            size_hint: None,None
-            font_size: 0
+            font_size: root.width / 4
+            opacity: 0
             icon: "check-circle"
             color: root.theme_cls.primary_color
 
     BoxLayout:
         size_hint_y: None
         height: dp(50)
         orientation: "vertical"
@@ -57,50 +57,47 @@
             theme_text_color: "Secondary"
             font_style: "Caption"
 """
 )
 
 
 class AKSelectListAvatarItem(
-    ThemableBehavior, ButtonBehavior, CircularRippleBehavior, BoxLayout
+    ThemableBehavior, CircularRippleBehavior, ButtonBehavior, BoxLayout
 ):
     columns = NumericProperty(4)
     source = StringProperty("")
     first_label = StringProperty("")
     second_label = StringProperty("")
     animate_start = BooleanProperty(True)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def _choose_selection(self, select):
-
         selected_list = self.parent._selected_list
 
         if select not in selected_list:
             selected_list.append(select)
             self._selection_anim()
 
         else:
             selected_list.remove(select)
             self._deselection_anim()
 
         if not selected_list:
             selected_list = []
-
         self.parent._selected_list = selected_list
 
     def _selection_anim(self):
-        anim = Animation(font_size=self.width / 3, t="out_bounce", duration=0.1)
+        anim = Animation(opacity=1, t="out_bounce", duration=0.1)
         anim.start(self.ids._box)
 
     def _deselection_anim(self):
         anim = Animation(
-            font_size=0,
-            size=self.ids._box.texture_size,
+            opacity=0,
             t="in_bounce",
             duration=0.1,
         )
         anim.start(self.ids._box)
 
 
 class AKSelectList(StackLayout):
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/silverappbar.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/silverappbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 adaptive_height: True
                 orientation: "vertical"
 
                 BoxLayout:
                     size_hint_y: None
                     height: root.max_height
 
-        MDToolbar:
+        MDTopAppBar:
             id: toolbar
             pos: self.x, float_box.height - self.height
             right_action_items: root.right_action_items
             left_action_items: root.left_action_items
             title: root.title
             anchor_title: root.anchor_title
             md_bg_color: root.toolbar_bg if root.toolbar_bg else root.theme_cls.primary_color
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/spinners.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/spinners.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/statusbarcolor.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/statusbarcolor.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/swipemenu.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/swipemenu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
-SwipeMenu
-=========
+Components/SwipeMenu
+====================
 
 Usage
 -----
 
 .. code-block:: python
 
     from kivy.lang.builder import Builder
-
     from kivymd.app import MDApp
-
-    import kivymd_extensions.akivymd
+    import kivymd_extensions.akivymd  # NOQA
 
     KV = '''
+
     <MyLabel@MDLabel>
         valign: 'center'
         halign: 'center'
         theme_text_color: "Custom"
         text_color: 1,1,1,1
 
-    Screen:
+
+    MDScreen:
 
         AKSwipeMenu:
 
             AKSwipeMenuMainContent:
                 MyLabel:
                     text: "Main Content"
                     text_color: 0,0,0,1
@@ -49,16 +49,18 @@
     '''
 
     class Test(MDApp):
 
         def build(self):
             return Builder.load_string(KV)
 
+
     Test().run()
 
+
 """
 
 
 from kivy.animation import Animation
 from kivy.event import EventDispatcher
 from kivy.lang.builder import Builder
 from kivy.properties import (
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/toolbar.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """
 Components/Toolbar
-=================
-
+==================
 
 Example
 -------
 
 .. code-block:: python
 
-    from kivy.uix.behaviors import ButtonBehavior
     from kivy.lang.builder import Builder
-
-    import kivymd_extensions.akivymd
+    from kivy.uix.behaviors import ButtonBehavior
     from kivymd.app import MDApp
     from kivymd.uix.list import OneLineListItem
 
+    import kivymd_extensions.akivymd  # NOQA
+
     kv = '''
 
-    Screen:
+    MDScreen:
 
         AKToolbarLayout:
             id: toolbar
 
             AKToolbarClass:
-                MDToolbar:
+                MDTopAppBar:
                     title: 'Hide On Scroll'
-                    left_action_items: [('menu', lambda x: None)]
+                    left_action_items: [['menu']]
 
             AKToolbarPinClass:
                 id: pin
                 height: dp(40)
                 canvas.before:
                     Color:
                         rgba: app.theme_cls.accent_color
@@ -50,23 +49,20 @@
                     icon: 'arrow-up'
                     on_release: toolbar.scroll_to(1)
 
     '''
 
 
     class Main(MDApp):
-
         def build(self):
             return Builder.load_string(kv)
 
         def on_start(self):
             for x in range(30):
-                self.root.ids.box.add_widget(OneLineListItem(
-                    text= f'List {x}'
-                ))
+                self.root.ids.box.add_widget(OneLineListItem(text=f"List {x}"))
             return super().on_start()
 
 
     Main().run()
 
 """
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/uix/windows.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/uix/windows.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,43 +9,43 @@
     ObjectProperty,
     StringProperty,
 )
 from kivy.uix.behaviors import ButtonBehavior
 from kivy.uix.boxlayout import BoxLayout
 from kivy.uix.floatlayout import FloatLayout
 from kivymd.theming import ThemableBehavior
-from kivymd.uix.behaviors import RectangularElevationBehavior
+from kivymd.uix.behaviors import CommonElevationBehavior
 
 Builder.load_string(
     """
 <HeaderButton>
     size_hint: None, None
     canvas.before:
         Color:
             rgba: root.button_color if root.button_color  else root.theme_cls.accent_color
         Ellipse:
             pos: self.pos
             size: self.size
 
     MDIcon:
         icon: root.button_icon
-        halign: "center"
-        valign: "center"
         theme_text_color: "Custom"
         text_color: root.button_text_color if root.button_text_color  else root.theme_cls.primary_color
         font_size: self.parent.height - dp(4)
         pos_hint: {"center_x": .5, "center_y": .5}
 
 
 <AKFloatingWindowLayout>
 
 
 <AKFloatingWindow>:
     orientation: "vertical"
     radius: [root.window_radius, ]
+    opacity: 0
+
     WindowHeader:
         orientation: "vertical"
         id: header
         size_hint_y: None
         height: root.header_height
         canvas.before:
             Color:
@@ -65,15 +65,17 @@
                 theme_text_color: "Custom"
                 text_color: root.header_text_color if root.header_text_color else 1, 1, 1, 1
 
             MDBoxLayout:
                 adaptive_width: True
                 spacing: dp(3)
                 padding: [dp(10), 0]
+
                 HeaderButton:
+                    opacity: 1 if root.allow_maximize else 0
                     size: header.height - dp(3), header.height - dp(3)
                     button_icon: root.max_button_icon
                     button_color: root.max_button_color if root.max_button_color else 0, 0, 1, 1
                     button_text_color: root.max_button_text_color if root.max_button_text_color else 1,1,1,1
                     pos_hint: {"center_x": .5, "center_y": .5}
                     on_release: root.maximize()
 
@@ -104,52 +106,56 @@
     pass
 
 
 class WindowContent(BoxLayout):
     pass
 
 
-class HeaderButton(ThemableBehavior, ButtonBehavior, BoxLayout):
+class HeaderButton(ThemableBehavior, ButtonBehavior, FloatLayout):
     button_icon = StringProperty()
     button_color = ListProperty()
     button_text_color = ListProperty()
 
 
 class AKFloatingWindow(
-    ThemableBehavior, RectangularElevationBehavior, BoxLayout
+    ThemableBehavior, CommonElevationBehavior, BoxLayout
 ):
     _window_active = BooleanProperty(False)
     header_height = NumericProperty("20dp")
     header_color_normal = ListProperty()
     header_color_active = ListProperty()
     header_text_color = ListProperty()
     title_font_size = NumericProperty("10dp")
     window_title = StringProperty()
-    window_elevation = NumericProperty(10)
+    window_elevation = NumericProperty(2)
     fade_exit = BooleanProperty(True)
     fade_open = BooleanProperty(True)
     animation_transition = StringProperty("out_quad")
     animation_duration = NumericProperty(0.1)
     open_position = ListProperty()
     maximize_animation = BooleanProperty(True)
     minimize_animation = BooleanProperty(True)
     window_radius = NumericProperty("8dp")
     bg_color = ListProperty()
+    minimum_window_width = NumericProperty("120dp")
+    minimum_window_height = NumericProperty("120dp")
 
     exit_button_icon = StringProperty("close")
     exit_button_color = ListProperty()
     exit_button_text_color = ListProperty()
     max_button_icon = StringProperty("window-maximize")
     max_button_color = ListProperty()
     max_button_text_color = ListProperty()
 
     bottom_widget = ObjectProperty()
     left_widget = ObjectProperty()
     right_widget = ObjectProperty()
     top_widget = ObjectProperty()
+    allow_resize = BooleanProperty(True)
+    allow_maximize = BooleanProperty(True)
 
     _state = "close"
     _maximized = False
     _resize_click_dis = NumericProperty("10dp")
     _allow_resize = False
     _size_before = False
     _pos_before = False
@@ -169,19 +175,16 @@
     def _update(self):
         if not self.header_color_active:
             self.header_color_active = self.theme_cls.primary_color
         if not self.header_color_normal:
             self.header_color_normal = self.theme_cls.primary_light
 
         self.elevation = self.window_elevation
-
-        exit_pos = [-self.width, -self.height]
-        self.pos = exit_pos
-        self.opacity = 0
         self._state = "close"
+        self.top = 0
 
     def _update_open_pos(self):
         self.open_position = [
             Window.size[0] / 2 - self.width / 2,
             Window.size[1] / 2 - self.height / 2,
         ]
 
@@ -248,14 +251,17 @@
             anim.start(self)
         else:
             self.pos = pos
             self.size = size
         self._maximized = False
 
     def maximize(self):
+        if not self.allow_maximize:
+            return
+
         if self._maximized:
             self.minimize_to_normal()
             return
 
         self._size_before = []
         self._pos_before = []
         self._size_before += [self.size[0], self.size[1]]
@@ -305,29 +311,46 @@
         right = window_right + self._resize_click_dis
         y = window_bottom - self._resize_click_dis
         top = window_bottom + self._resize_click_dis
 
         if x < touch_pos[0] < right and y < touch_pos[1] < top:
             self._allow_resize = True
             Window.set_system_cursor("size_nwse")
+
+        if self.collide_point(*touch.pos):
+            for child in self.children:
+                child.on_touch_down(touch)
+            return True
+
         return super().on_touch_down(touch)
 
     def on_touch_up(self, touch):
         self._allow_resize = False
         Window.set_system_cursor("arrow")
         return super().on_touch_up(touch)
 
     def on_touch_move(self, touch):
-        if self._allow_resize:
+        if self._allow_resize and self.allow_resize:
             touch_pos = touch.pos
 
             width = touch_pos[0] - self.x
             height = self.y + self.height - touch_pos[1]
+            if (
+                width < self.minimum_window_width
+                or height < self.minimum_window_height
+            ):
+                return True
             self.size = [width, height]
             self.pos = [self.x, touch_pos[1]]
+            return True
+
+        if self.collide_point(*touch.pos):
+            for child in self.children:
+                child.on_touch_down(touch)
+            return True
 
         return super().on_touch_move(touch)
 
 
 class AKFloatingWindowLayout(ThemableBehavior, FloatLayout):
     _allow_move = False
     _x_dist = None
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions/akivymd/utils/draw_tools.py` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions/akivymd/utils/draw_tools.py`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/PKG-INFO` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,16 @@
 Metadata-Version: 2.1
 Name: kivymd-extensions.akivymd
-Version: 1.2.6
+Version: 1.2.7
 Summary: A set of fancy widgets for KivyMD
 Home-page: https://github.com/kivymd-extensions/akivymd
 Author: quitegreensky, KivyMD Team and other contributors
 Author-email: quitegreensky@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/kivymd-extensions/akivymd/issues
-Description: # Awesome KivyMD
-        
-        Awesome KivyMD is a package containing customized and non-material widgets for KivyMD.
-        
-        <p align="center">
-            <img align="center" width="512" src="https://raw.githubusercontent.com/quitegreensky/akivymd/master/images/preview.gif"/>
-        </p>
-        
-        ## Installation
-        
-        ```bash
-        pip install kivymd_extensions.akivymd
-        
-        #or 
-        
-        pip install https://github.com/kivymd-extensions/akivymd/archive/main.zip
-        ```
-        
-        ## Usage with Buildozer
-        
-        ```bash
-        requirements = https://github.com/kivymd-extensions/akivymd/archive/main.zip
-        ```
-        
-        ### Dependencies:
-        
-        - [KivyMD](https://github.com/kivymd/KivyMD) >= 0.104.2 (from master branch)
-        - [Kivy](https://github.com/kivy/kivy) >= 1.11.1 ([Installation](https://kivy.org/doc/stable/gettingstarted/installation.html))
-        - [Python 3.6+](https://www.python.org/)
-        
-        ## Documentation
-        
-        ### Usage
-        
-        ```python
-        from kivy.lang import Builder
-        
-        from kivymd.app import MDApp
-        import kivymd_extensions.akivymd
-        
-        KV = """
-        <NavigationButton@Button_Item>
-            icon_color: app.theme_cls.text_color
-            text_color: app.theme_cls.text_color
-            button_bg_color: app.theme_cls.primary_color
-            mode: 'color_on_active'
-            badge_disabled: True
-        
-        
-        MDScreen:
-        
-            AKBottomNavigation2:
-                bg_color: app.theme_cls.bg_darkest
-                
-                NavigationButton:
-                    text: 'Alert'
-                    icon: 'bell-outline'
-                
-                NavigationButton:
-                    text: 'Bank'
-                    icon: 'bank-outline'
-                
-                NavigationButton:
-                    text: 'Download'
-                    icon: 'arrow-down-bold-outline'
-        """
-        
-        
-        class Test(MDApp):
-            def build(self):
-                return Builder.load_string(KV)
-        
-        
-        Test().run()
-        ```
-        
-        ## Examples
-        
-        ```bash
-        git clone https://github.com/kivymd-extensions/akivymd.git
-        cd akivymd
-        cd examples/full_example
-        python main.py
-        ```
-        
-        ## Support
-        
-        If you need assistance or you have a question, you can ask for help on our mailing list:
-        
-        - **Discord server:** https://discord.gg/wu3qBST
-        - _Email:_ kivydevelopment@gmail.com
-        
-        ## License
-        
-        [MIT License](LICENSE)
-        
 Keywords: kivymd_extensions,kivymd,kivy,material,ui
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -127,11 +31,116 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
+
+# Awesome KivyMD
+
+Awesome KivyMD is a package containing customized and non-material widgets for KivyMD.
+
+<p align="center">
+    <img align="center" width="512" src="https://raw.githubusercontent.com/quitegreensky/akivymd/master/images/preview.gif"/>
+</p>
+
+## Installation
+
+```bash
+pip install kivymd_extensions.akivymd
+
+#or
+
+pip install https://github.com/kivymd-extensions/akivymd/archive/main.zip
+```
+
+## Usage with Buildozer
+
+```bash
+requirements = https://github.com/kivymd-extensions/akivymd/archive/main.zip
+```
+
+### Dependencies:
+
+- [KivyMD](https://github.com/kivymd/KivyMD) >= 0.104.2 (from master branch)
+- [Kivy](https://github.com/kivy/kivy) >= 1.11.1 ([Installation](https://kivy.org/doc/stable/gettingstarted/installation.html))
+- [Python 3.6+](https://www.python.org/)
+
+## Documentation
+
+### Usage
+
+```python
+from kivy.lang import Builder
+
+from kivymd.app import MDApp
+import kivymd_extensions.akivymd
+
+KV = """
+<NavigationButton@Button_Item>
+    icon_color: app.theme_cls.text_color
+    text_color: app.theme_cls.text_color
+    button_bg_color: app.theme_cls.primary_color
+    mode: 'color_on_active'
+    badge_disabled: True
+
+
+MDScreen:
+
+    AKBottomNavigation2:
+        bg_color: app.theme_cls.bg_darkest
+
+        NavigationButton:
+            text: 'Alert'
+            icon: 'bell-outline'
+
+        NavigationButton:
+            text: 'Bank'
+            icon: 'bank-outline'
+
+        NavigationButton:
+            text: 'Download'
+            icon: 'arrow-down-bold-outline'
+"""
+
+
+class Test(MDApp):
+    def build(self):
+        return Builder.load_string(KV)
+
+
+Test().run()
+```
+
+## Examples
+
+```bash
+git clone https://github.com/kivymd-extensions/akivymd.git
+cd akivymd
+cd examples/full_example
+python main.py
+```
+
+## Build Docs
+
+```bash
+git clone https://github.com/kivymd-extensions/akivymd.git
+cd docs
+sphinx-build -b html sources ./_build
+```
+
+## Support
+
+If you need assistance or you have a question, you can ask for help on our mailing list:
+
+- **Discord server:** https://discord.gg/wu3qBST
+- _Email:_ kivydevelopment@gmail.com
+
+## License
+
+[MIT License](LICENSE)
```

### Comparing `kivymd_extensions.akivymd-1.2.6/kivymd_extensions.akivymd.egg-info/SOURCES.txt` & `kivymd_extensions.akivymd-1.2.7/kivymd_extensions.akivymd.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 kivymd_extensions/akivymd/factory_registers.py
 kivymd_extensions/akivymd/helper.py
 kivymd_extensions/akivymd/uix/__init__.py
 kivymd_extensions/akivymd/uix/badgelayout.py
 kivymd_extensions/akivymd/uix/bottomappbar.py
 kivymd_extensions/akivymd/uix/bottomnavigation.py
 kivymd_extensions/akivymd/uix/bottomnavigation2.py
+kivymd_extensions/akivymd/uix/buttonpanel.py
+kivymd_extensions/akivymd/uix/cardstack.py
 kivymd_extensions/akivymd/uix/charts.py
 kivymd_extensions/akivymd/uix/datepicker.py
 kivymd_extensions/akivymd/uix/dialogs.py
 kivymd_extensions/akivymd/uix/hintwidget.py
 kivymd_extensions/akivymd/uix/imageview.py
 kivymd_extensions/akivymd/uix/loaders.py
 kivymd_extensions/akivymd/uix/navigationrail.py
```

### Comparing `kivymd_extensions.akivymd-1.2.6/pyproject.toml` & `kivymd_extensions.akivymd-1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/setup.cfg` & `kivymd_extensions.akivymd-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `kivymd_extensions.akivymd-1.2.6/setup.py` & `kivymd_extensions.akivymd-1.2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,11 +49,11 @@
             ],
             "docs": [
                 "sphinx",
                 "sphinx-autoapi==1.4.0",
                 "sphinx_rtd_theme",
             ],
         },
-        install_requires=["kivymd>=0.104.1", "kivy>=1.11.1"],
+        install_requires=["kivymd>=1.1.1", "kivy>=2.2.1"],
         setup_requires=[],
-        python_requires=">=3.6",
+        python_requires=">=3.7",
     )
```

