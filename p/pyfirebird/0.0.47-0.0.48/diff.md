# Comparing `tmp/pyfirebird-0.0.47.tar.gz` & `tmp/pyfirebird-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.47.tar", last modified: Mon Jun 26 09:33:16 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.48.tar", last modified: Tue Jun 27 20:39:11 2023, max compression
```

## Comparing `pyfirebird-0.0.47.tar` & `pyfirebird-0.0.48.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.47/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1301 2023-05-13 19:27:50.000000 pyfirebird-0.0.47/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-06-26 09:30:30.000000 pyfirebird-0.0.47/src/firebird/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.47/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/cmd_tools/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2551 2023-06-26 09:30:32.000000 pyfirebird-0.0.47/src/firebird/cmd_tools/executor.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     4715 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/cmd_tools/executor_impl.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/cmd_tools/fbconsole.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2653 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/cmd_tools/pipeline.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     1866 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/cmd_tools/pipeline_impl.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/rabbitmq.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebird/utils/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/utils/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.47/src/firebird/utils/checkpoint.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     6163 2023-06-26 09:30:30.000000 pyfirebird-0.0.47/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/asgi.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/settings.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/wsgi.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebirdconsole/ui/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/admin.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/apps.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebirdconsole/ui/migrations/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/migrations/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-26 09:30:33.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/models.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebirdconsole/ui/static/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.876696 pyfirebird-0.0.47/src/firebirdconsole/ui/static/images/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/static/images/logo.jpeg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1554534 2023-06-26 09:30:38.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/home.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1676441 2023-06-26 09:32:29.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/pipeline.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/src/firebirdconsole/ui/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/templates/application.html
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/templates/index.html
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/src/firebirdconsole/ui/templatetags/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/templatetags/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/templatetags/app_filters.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/tests.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      473 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/view_tools.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/src/firebirdconsole/ui/views/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/views/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/src/firebirdconsole/ui/views/apis/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/views/apis/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3939 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/views/apis/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/views/home.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.47/src/firebirdconsole/ui/views/pipeline.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:33:16.880697 pyfirebird-0.0.47/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-06-26 09:33:16.000000 pyfirebird-0.0.47/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1833 2023-06-26 09:33:16.000000 pyfirebird-0.0.47/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-06-26 09:33:16.000000 pyfirebird-0.0.47/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:33:16.000000 pyfirebird-0.0.47/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       70 2023-06-26 09:33:16.000000 pyfirebird-0.0.47/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-06-26 09:33:16.000000 pyfirebird-0.0.47/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.48/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1293 2023-06-27 18:17:58.000000 pyfirebird-0.0.48/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-06-26 09:30:30.000000 pyfirebird-0.0.48/src/firebird/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.48/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.48/src/firebird/cmd_tools/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2551 2023-06-27 19:59:58.000000 pyfirebird-0.0.48/src/firebird/cmd_tools/executor.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4715 2023-06-27 18:39:03.000000 pyfirebird-0.0.48/src/firebird/cmd_tools/executor_impl.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.48/src/firebird/cmd_tools/fbconsole.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3457 2023-06-27 20:34:56.000000 pyfirebird-0.0.48/src/firebird/cmd_tools/pipeline.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2045 2023-06-27 20:27:53.000000 pyfirebird-0.0.48/src/firebird/cmd_tools/pipeline_impl.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.48/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.48/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.48/src/firebird/utils/checkpoint.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6688 2023-06-27 19:56:54.000000 pyfirebird-0.0.48/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/asgi.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/settings.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/wsgi.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebirdconsole/ui/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/admin.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/apps.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebirdconsole/ui/migrations/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/migrations/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-26 09:30:33.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/models.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.872083 pyfirebird-0.0.48/src/firebirdconsole/ui/static/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.876083 pyfirebird-0.0.48/src/firebirdconsole/ui/static/images/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/static/images/logo.jpeg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1554534 2023-06-27 08:39:24.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/home.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1676441 2023-06-27 08:39:24.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/pipeline.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/src/firebirdconsole/ui/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/templates/application.html
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/templates/index.html
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/src/firebirdconsole/ui/templatetags/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/templatetags/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/templatetags/app_filters.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/tests.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      473 2023-06-27 08:39:24.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/view_tools.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/src/firebirdconsole/ui/views/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/views/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/src/firebirdconsole/ui/views/apis/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-27 08:39:24.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/views/apis/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3939 2023-06-27 08:39:24.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/views/apis/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/views/home.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.48/src/firebirdconsole/ui/views/pipeline.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-27 20:39:11.880083 pyfirebird-0.0.48/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-06-27 20:39:11.000000 pyfirebird-0.0.48/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1833 2023-06-27 20:39:11.000000 pyfirebird-0.0.48/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-06-27 20:39:11.000000 pyfirebird-0.0.48/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-27 20:39:11.000000 pyfirebird-0.0.48/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       65 2023-06-27 20:39:11.000000 pyfirebird-0.0.48/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-06-27 20:39:11.000000 pyfirebird-0.0.48/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.47/setup.py` & `pyfirebird-0.0.48/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.47",
+    version="0.0.48",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
@@ -23,15 +23,15 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     package_dir = {'': 'src'},
     packages=find_packages(where='src'),
     package_data={"firebirdconsole": ["ui/templates/*", "ui/static/js-bundle/*", "ui/static/images/*"]},
     include_package_data=True,
-    install_requires=["pika", "kazoo", "docker", "paramiko", "Django>=4.2.1", "mysqlclient", "graphviz>=0.20.1"],
+    install_requires=["pika", "kazoo", "Django>=4.2.1", "mysqlclient", "graphviz>=0.20.1", "kubernetes"],
     entry_points={
         "console_scripts": [
             "pipeline=firebird.cmd_tools.pipeline:main",
             "executor=firebird.cmd_tools.executor:main",
             "fbconsole=firebird.cmd_tools.fbconsole:main",
         ]
     },
```

### Comparing `pyfirebird-0.0.47/src/firebird/base.py` & `pyfirebird-0.0.48/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.48/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebird/cmd_tools/executor_impl.py` & `pyfirebird-0.0.48/src/firebird/cmd_tools/executor_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebird/cmd_tools/fbconsole.py` & `pyfirebird-0.0.48/src/firebird/cmd_tools/fbconsole.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.48/src/firebird/cmd_tools/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,14 +28,20 @@
         "handlers": ["console"],
         "level": "DEBUG",
     },
 }
 
 # logger = logging.getLogger(__name__)
 
+def check_args(args, names):
+    for name in names:
+        if getattr(args, name) is None:
+            print(f"Missing option --{name.repalce("_", "-")}")
+            sys.exit(2)
+
 def main():
     parser = argparse.ArgumentParser(
         description='Pipeline Tool'
     )
     parser.add_argument(
         "action", type=str, help="Specify action",
         choices=['register', 'unregister', 'list', 'stop'],
@@ -58,14 +64,20 @@
         "-pid", "--pipeline-id", type=str, required=False, help="pipeline ID"
     )
     parser.add_argument(
         "-wc", "--worker-count", type=int, default=1, required=False,
         help="Worker count"
     )
     parser.add_argument(
+        "-pnn", "--pipeline-namespace-name", type=str, required=False, help="pipeline namespace name"
+    )
+    parser.add_argument(
+        "-pin", "--pipeline-image-name", type=str, required=False, help="pipeline image name"
+    )
+    parser.add_argument(
         "-eid", "--executor-id", type=str, required=False, help="Executor ID"
     )
     args = parser.parse_args()
     action = args.action[0]
 
     if args.debug:
         logging.config.dictConfig(LOG_CONFIG)
@@ -78,19 +90,29 @@
 
     with open(config_filename, "rt") as f:
         config = json.load(f)
 
     impl = importlib.import_module("firebird.cmd_tools.pipeline_impl")
 
     if action == "register":
-        impl.register_command(config, args.pipeline_module_name)
+        check_args(["pipeline_namespace_name", "pipeline_image_name", "pipeline_module_name"])
+        impl.register_command(
+            config, 
+            args.pipeline_namespace_name, 
+            args.pipeline_image_name, 
+            args.pipeline_module_name
+        )
     if action == "unregister":
+        check_args(["pipeline_id"])
         impl.unregister_command(config, args.pipeline_id)
     elif action == "list":
         impl.list_command(config)
+    elif action == "start":
+        check_args(["pipeline_id"])
+        impl.start_command(config, args.pipeline_id)
     elif action == "stop":
         impl.stop_command(config, args.pipeline_id, args.executor_id)
         
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyfirebird-0.0.47/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.48/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from typing import Dict, Callable
 import logging
 import logging.config
 import importlib
 from uuid import uuid4
 from firebird.rabbitmq import get_connection, RabbitMQ
 from firebird import zkdb
-import docker
+from kubernetes import client, config
 
 logger = logging.getLogger(__name__)
 
-def register_command(config:dict, pipeline_module_name:str):
+def register_command(config:dict, pipeline_namespace_name:str, pipeline_image_name:str, pipeline_module_name:str):
     pipeline = importlib.import_module(pipeline_module_name).get_pipeline(None)
     pipeline_info = pipeline.to_json()
 
     mq = RabbitMQ(
         connection = get_connection(**config["rabbitmq"]),
         topic = pipeline.id
     )
     # create rabbitmq topic, etc
     mq.initialize()
 
     with zkdb(**config['zookeeper']) as db:
-        db.register_pipeline(pipeline.id, pipeline_module_name, pipeline_info)
+        db.register_pipeline(pipeline.id, pipeline_namespace_name, pipeline_image_name, pipeline_module_name)
 
 def unregister_command(config:dict, pipeline_id:str):
     with zkdb(**config['zookeeper']) as db:
         db.unregister_pipeline(pipeline_id)
 
 def list_command(config):
     with zkdb(**config['zookeeper']) as db:
@@ -47,7 +47,10 @@
                 print(f"            start_time            = {executor_info['start_time']}")
                 print(f"            pid                   = {executor_info['pid']}")
 
 def stop_command(config:dict, pipeline_id:str, executor_id:str):
     with zkdb(**config['zookeeper']) as db:
         db.stop_executor(pipeline_id, executor_id)
 
+
+def start_command(config, pipeline_id):
+    print("Not implemented")
```

### Comparing `pyfirebird-0.0.47/src/firebird/rabbitmq.py` & `pyfirebird-0.0.48/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebird/utils/checkpoint.py` & `pyfirebird-0.0.48/src/firebird/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebird/zkdb.py` & `pyfirebird-0.0.48/src/firebird/zkdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,26 +18,28 @@
 class ZKDatabase:
     """
     Manage zookeeper database
     """
     def __init__(self, zk):
         self.zk = zk
     
-    def register_pipeline(self, pipeline_id:str, pipeline_module_name:str, pipeline_info:str):
+    def register_pipeline(self, pipeline_id:str, pipeline_namespace_name:str, pipeline_image_name:str, pipeline_module_name:str, pipeline_info:str):
         """
         Register a pipeline
         """
         self.zk.ensure_path("/pipelines")
         pipeline_path = f"/pipelines/{pipeline_id}"
         if self.zk.exists(pipeline_path):
             raise Exception(f"Pipeline {pipeline_id} is already registered!")
         
         self.zk.ensure_path(pipeline_path)
         self.zk.create(f"{pipeline_path}/info", json.dumps(pipeline_info).encode("utf-8"))
         self.zk.create(f"{pipeline_path}/module", pipeline_module_name.encode("utf-8"))
+        self.zk.create(f"{pipeline_path}/namespace", pipeline_namespace_name.encode("utf-8"))
+        self.zk.create(f"{pipeline_path}/image_name", pipeline_image_name.encode("utf-8"))
 
     def unregister_pipeline(self, pipeline_id:str):
         """
         Unregister a pipeline
         """
         pipeline_path = f"/pipelines/{pipeline_id}"
         if not self.zk.exists(pipeline_path):
@@ -92,25 +94,31 @@
         if not self.zk.exists(pipeline_path):
             return None
 
         v, _ = self.zk.get(f"{pipeline_path}/info")
         pipeline_info = json.loads(v.decode("utf-8"))
         v, _ = self.zk.get(f"{pipeline_path}/module")
         module = v.decode("utf-8")
+        v, _ = self.zk.get(f"{pipeline_path}/namespace_name")
+        namespace_name = v.decode("utf-8")
+        v, _ = self.zk.get(f"{pipeline_path}/image_name")
+        image_name = v.decode("utf-8")
 
         executor_ids_path = f"/pipelines/{pipeline_id}/executors"
         executors = []
         if self.zk.exists(executor_ids_path):
             executors = [
                 self.get_executor(pipeline_id, executor_id) for executor_id in self.zk.get_children(executor_ids_path)
             ]
         
         return {
             "info": pipeline_info,
             "module": module,
+            "image_name": image_name,
+            "namespace_name": namespace_name,
             "executors": executors
         }
 
 
     def register_executor(
         self, 
         pipeline_id:str,
```

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/settings.py` & `pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/settings.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/firebirdconsole/urls.py` & `pyfirebird-0.0.48/src/firebirdconsole/firebirdconsole/urls.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/static/images/logo.jpeg` & `pyfirebird-0.0.48/src/firebirdconsole/ui/static/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/home.js` & `pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/home.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/pipeline.js` & `pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/pipeline.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt` & `pyfirebird-0.0.48/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/templates/application.html` & `pyfirebird-0.0.48/src/firebirdconsole/ui/templates/application.html`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/templatetags/app_filters.py` & `pyfirebird-0.0.48/src/firebirdconsole/ui/templatetags/app_filters.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/view_tools.py` & `pyfirebird-0.0.48/src/firebirdconsole/ui/view_tools.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/firebirdconsole/ui/views/apis/main.py` & `pyfirebird-0.0.48/src/firebirdconsole/ui/views/apis/main.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.47/src/pyfirebird.egg-info/SOURCES.txt` & `pyfirebird-0.0.48/src/pyfirebird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

