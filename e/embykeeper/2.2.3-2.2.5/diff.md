# Comparing `tmp/embykeeper-2.2.3.tar.gz` & `tmp/embykeeper-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.3.tar", last modified: Mon Jun 26 05:16:06 2023, max compression
+gzip compressed data, was "embykeeper-2.2.5.tar", last modified: Mon Jun 26 23:47:53 2023, max compression
```

## Comparing `embykeeper-2.2.3.tar` & `embykeeper-2.2.5.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 05:15:52.000000 embykeeper-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 05:15:52.000000 embykeeper-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-06-26 05:16:06.983669 embykeeper-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-06-26 05:15:52.000000 embykeeper-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/css/cascadia-code.css
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 05:15:52.000000 embykeeper-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:16:06.983669 embykeeper-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-26 05:15:52.000000 embykeeper-2.2.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.205008 embykeeper-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 23:47:40.000000 embykeeper-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 23:47:40.000000 embykeeper-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23799 2023-06-26 23:47:53.205008 embykeeper-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-06-26 23:47:40.000000 embykeeper-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.189008 embykeeper-2.2.5/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.193008 embykeeper-2.2.5/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.193008 embykeeper-2.2.5/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.197008 embykeeper-2.2.5/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.197008 embykeeper-2.2.5/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.197008 embykeeper-2.2.5/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.193008 embykeeper-2.2.5/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23799 2023-06-26 23:47:53.000000 embykeeper-2.2.5/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-26 23:47:53.000000 embykeeper-2.2.5/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:47:53.000000 embykeeper-2.2.5/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 23:47:53.000000 embykeeper-2.2.5/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:47:52.000000 embykeeper-2.2.5/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 23:47:53.000000 embykeeper-2.2.5/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 23:47:53.000000 embykeeper-2.2.5/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.189008 embykeeper-2.2.5/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.189008 embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/css/cascadia-code.css
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.189008 embykeeper-2.2.5/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-26 23:47:40.000000 embykeeper-2.2.5/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 23:47:40.000000 embykeeper-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 23:47:53.205008 embykeeper-2.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:47:53.201008 embykeeper-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-26 23:47:40.000000 embykeeper-2.2.5/tests/test_cli.py
```

### Comparing `embykeeper-2.2.3/LICENSE` & `embykeeper-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/PKG-INFO` & `embykeeper-2.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.3
+Version: 2.2.5
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -36,38 +36,38 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/7Q7MzwYT) 获得社区帮助.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
 
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+    - ~~EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~ (停止签到)
 - Emby 保活
 
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
 
   - 默认禁用:
@@ -98,14 +98,18 @@
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
 
+#### 其他免费 Pass
+
+您也可以通过 [Patr.cloud](https://app.patr.cloud/) ([教程](https://blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) 等平台进行部署.
+
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
@@ -412,15 +416,19 @@
 
 ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
 
 ![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
 
 ## 代码重用与开发
 
-代码架构如下:
+您可以查看 [CONTRIBUTING](https://github.com/embykeeper/embykeeper/blob/main/CONTRIBUTING.md) 以了解如何贡献代码.
+
+您也可以通过 [Discord](https://discord.gg/a4bmY38u) 参与开发讨论.
+
+项目代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
     A --> C(fa:fa-play embywatcher)
     B --checker--> E[fa:fa-robot Bot]
     B --monitor--> G[fa:fa-eye Monitor]
@@ -483,14 +491,23 @@
 请输入各群组最大获取数量 [1000]:
 ```
 
 该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
 
 另一个工具是即时信息分析:
 
+<!--
+;    用户             会话   (ChatID)                发信人   (UserID)                      信息
+; ────────────────────────────────────────────────────────────────────────────────────────────────────────────
+;   Tester  │  👥 Group A  -1001464166237   │   🤖 Bot A   1965142520   │  Welcome to the bar, what to drink?
+;   Tester  │  👥 Group A  -1001464166237   │   👤 User A  749799257    │  I want -1 cup of beer.
+;   Tester  │  👥 Group A  -1001464166237   │   👤 User B  749799257    │  A dish of asdfQwer@24dg!&*(@.
+;   Tester  │  👥 Group A  -1001464166237   │   🤖 Bot A   1965142520   │  Boom.
+-->
+
 ![follow screenshot](images/follow.svg)
 
 该工具可以实时输出消息的 ID 等信息, 以方便调试.
 
 ## 趋势
 
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.3 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.5 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -39,14 +39,15 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
+æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/7Q7MzwYT) è·å¾ç¤¾åºå¸®å©.
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
@@ -56,26 +57,26 @@
 t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
 (https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
 (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
 t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
 Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
 [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
 peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
-t.me/peach_emby_bot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https:/
-/t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Pornemby: [é¢é](https://
-t.me/pornembyservice) [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/
-PronembyTGBot2_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
-[æºå¨äºº](https://t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV)
-[ç¾¤ç»](https://t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) -
-å¶ä»é Emby ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/
-embykeeper/pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-~~BlueSea: [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/
-blueseamusic_bot)~~ (æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
-CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
-t.me/JMSIPTV_bot)~~ (æ ååº) - Emby ä¿æ´» -
+t.me/peach_emby_bot) - Pornemby: [é¢é](https://t.me/pornembyservice)
+[ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
+åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
+pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: - ~~BlueSea:
+[ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~
+(æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
+(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~
+(æ ååº) - ~~EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
+emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ (åæ­¢ç­¾å°) - Emby ä¿æ´» -
 å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
 èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
@@ -100,20 +101,22 @@
 é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
-å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». ### éè¿ Docker é¨ç½² Embykeeper
-å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://yeasy.gitbook.io/
-docker_practice/install), ç¶åæ§è¡: ```bash docker run -v $(pwd)/
-embykeeper:/app --rm -it --net=host embykeeper/embykeeper ``` å½ä»¤å°ä¼å¨
-`embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
+æ¨ä¹å¯ä»¥éè¿ [Patr.cloud](https://app.patr.cloud/) ([æç¨](https://
+blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) ç­å¹³å°è¿è¡é¨ç½². ###
+éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£
+docker](https://yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡:
+```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/
+embykeeper ``` å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml`
+æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
 (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
 "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
 `config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
 port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
 run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
@@ -249,20 +252,23 @@
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
-embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å
-ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
-telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
-Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
-``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
+embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å æ¨å¯ä»¥æ¥ç
+[CONTRIBUTING](https://github.com/embykeeper/embykeeper/blob/main/
+CONTRIBUTING.md) ä»¥äºè§£å¦ä½è´¡ç®ä»£ç . æ¨ä¹å¯ä»¥éè¿ [Discord]
+(https://discord.gg/a4bmY38u) åä¸å¼åè®¨è®º. é¡¹ç®ä»£ç æ¶æå¦ä¸:
+```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
+A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-robot Bot] B --monitor--
+> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message Messager] C --watcher--
+> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A ```
+ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
 `embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
 éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
 = 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
 "`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
 è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
@@ -278,11 +284,11 @@
 å¼åå·¥å· æ¨å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
 ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
 config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
 10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
 "åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
 è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
-å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
+å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ:  ![follow screenshot](images/follow.svg)
 è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ## è¶å¿
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
 embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.2.3/README.md` & `embykeeper-2.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,38 +15,38 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/7Q7MzwYT) 获得社区帮助.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
 
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+    - ~~EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~ (停止签到)
 - Emby 保活
 
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
 
   - 默认禁用:
@@ -77,14 +77,18 @@
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
 
+#### 其他免费 Pass
+
+您也可以通过 [Patr.cloud](https://app.patr.cloud/) ([教程](https://blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) 等平台进行部署.
+
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
@@ -391,15 +395,19 @@
 
 ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
 
 ![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
 
 ## 代码重用与开发
 
-代码架构如下:
+您可以查看 [CONTRIBUTING](https://github.com/embykeeper/embykeeper/blob/main/CONTRIBUTING.md) 以了解如何贡献代码.
+
+您也可以通过 [Discord](https://discord.gg/a4bmY38u) 参与开发讨论.
+
+项目代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
     A --> C(fa:fa-play embywatcher)
     B --checker--> E[fa:fa-robot Bot]
     B --monitor--> G[fa:fa-eye Monitor]
@@ -462,14 +470,23 @@
 请输入各群组最大获取数量 [1000]:
 ```
 
 该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
 
 另一个工具是即时信息分析:
 
+<!--
+;    用户             会话   (ChatID)                发信人   (UserID)                      信息
+; ────────────────────────────────────────────────────────────────────────────────────────────────────────────
+;   Tester  │  👥 Group A  -1001464166237   │   🤖 Bot A   1965142520   │  Welcome to the bar, what to drink?
+;   Tester  │  👥 Group A  -1001464166237   │   👤 User A  749799257    │  I want -1 cup of beer.
+;   Tester  │  👥 Group A  -1001464166237   │   👤 User B  749799257    │  A dish of asdfQwer@24dg!&*(@.
+;   Tester  │  👥 Group A  -1001464166237   │   🤖 Bot A   1965142520   │  Boom.
+-->
+
 ![follow screenshot](images/follow.svg)
 
 该工具可以实时输出消息的 ID 等信息, 以方便调试.
 
 ## 趋势
 
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -27,14 +27,15 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
+æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/7Q7MzwYT) è·å¾ç¤¾åºå¸®å©.
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
@@ -44,26 +45,26 @@
 t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
 (https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
 (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
 t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
 Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
 [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
 peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
-t.me/peach_emby_bot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https:/
-/t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Pornemby: [é¢é](https://
-t.me/pornembyservice) [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/
-PronembyTGBot2_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
-[æºå¨äºº](https://t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV)
-[ç¾¤ç»](https://t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) -
-å¶ä»é Emby ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/
-embykeeper/pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-~~BlueSea: [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/
-blueseamusic_bot)~~ (æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
-CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
-t.me/JMSIPTV_bot)~~ (æ ååº) - Emby ä¿æ´» -
+t.me/peach_emby_bot) - Pornemby: [é¢é](https://t.me/pornembyservice)
+[ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
+åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
+pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: - ~~BlueSea:
+[ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~
+(æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
+(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~
+(æ ååº) - ~~EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
+emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ (åæ­¢ç­¾å°) - Emby ä¿æ´» -
 å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
 èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
@@ -88,20 +89,22 @@
 é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
-å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». ### éè¿ Docker é¨ç½² Embykeeper
-å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://yeasy.gitbook.io/
-docker_practice/install), ç¶åæ§è¡: ```bash docker run -v $(pwd)/
-embykeeper:/app --rm -it --net=host embykeeper/embykeeper ``` å½ä»¤å°ä¼å¨
-`embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
+æ¨ä¹å¯ä»¥éè¿ [Patr.cloud](https://app.patr.cloud/) ([æç¨](https://
+blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) ç­å¹³å°è¿è¡é¨ç½². ###
+éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£
+docker](https://yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡:
+```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/
+embykeeper ``` å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml`
+æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
 (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
 "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
 `config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
 port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
 run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
@@ -237,20 +240,23 @@
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
-embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å
-ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
-telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
-Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
-``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
+embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å æ¨å¯ä»¥æ¥ç
+[CONTRIBUTING](https://github.com/embykeeper/embykeeper/blob/main/
+CONTRIBUTING.md) ä»¥äºè§£å¦ä½è´¡ç®ä»£ç . æ¨ä¹å¯ä»¥éè¿ [Discord]
+(https://discord.gg/a4bmY38u) åä¸å¼åè®¨è®º. é¡¹ç®ä»£ç æ¶æå¦ä¸:
+```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
+A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-robot Bot] B --monitor--
+> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message Messager] C --watcher--
+> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A ```
+ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
 `embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
 éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
 = 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
 "`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
 è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
@@ -266,11 +272,11 @@
 å¼åå·¥å· æ¨å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
 ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
 config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
 10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
 "åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
 è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
-å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
+å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ:  ![follow screenshot](images/follow.svg)
 è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ## è¶å¿
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
 embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.2.3/embykeeper/cli.py` & `embykeeper-2.2.5/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/data.py` & `embykeeper-2.2.5/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.5/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/embywatcher/main.py` & `embykeeper-2.2.5/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/log.py` & `embykeeper-2.2.5/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/settings.py` & `embykeeper-2.2.5/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.5/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/link.py` & `embykeeper-2.2.5/embykeeper/telechecker/link.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,58 +36,57 @@
                 self.log.debug(f"[gray50]删除了API消息记录: {text}[/]")
             except asyncio.CancelledError:
                 pass
 
         return await asyncio.gather(*[delete(m) for m in messages])
 
     async def post(
-        self, cmd, condition: Callable = None, timeout: int = 10, name: str = None
+        self, cmd, condition: Callable = None, timeout: int = 5, retries=3, name: str = None
     ) -> Tuple[Optional[str], Optional[str]]:
-        self.log.debug(f"[gray50]禁用提醒 {timeout} 秒: {self.bot}[/]")
-        await self.client.mute_chat(self.bot, time.time() + timeout + 5)
-        future = asyncio.Future()
-        handler = MessageHandler(
-            async_partial(self._handler, cmd=cmd, future=future, condition=condition),
-            filters.text & filters.bot & filters.user(self.bot),
-        )
-        groups = self.client.dispatcher.groups
-        if 1 not in groups:
-            groups[1] = [handler]
-        else:
-            groups[1].append(handler)
-        messages = []
-        messages.append(await self.client.send_message(self.bot, f"/start quiet"))
-        await asyncio.sleep(0.5)
-        messages.append(await self.client.send_message(self.bot, cmd))
-        try:
-            results = await asyncio.wait_for(future, timeout=timeout)
-        except asyncio.CancelledError:
+        for _ in range(retries):
+            self.log.debug(f"[gray50]禁用提醒 {timeout} 秒: {self.bot}[/]")
+            await self.client.mute_chat(self.bot, time.time() + timeout + 5)
+            future = asyncio.Future()
+            handler = MessageHandler(
+                async_partial(self._handler, cmd=cmd, future=future, condition=condition),
+                filters.text & filters.bot & filters.user(self.bot),
+            )
+            self.client.add_handler(handler, group=1)
             try:
-                await asyncio.wait_for(self.delete_messages(messages), 1.0)
+                messages = []
+                messages.append(await self.client.send_message(self.bot, f"/start quiet"))
+                await asyncio.sleep(0.5)
+                messages.append(await self.client.send_message(self.bot, cmd))
+                results = await asyncio.wait_for(future, timeout=timeout)
+            except asyncio.CancelledError:
+                try:
+                    await asyncio.wait_for(self.delete_messages(messages), 1.0)
+                except asyncio.TimeoutError:
+                    pass
+                finally:
+                    raise
             except asyncio.TimeoutError:
-                pass
+                await self.delete_messages(messages)
+                self.log.warning(f"{name}超时.")
+                continue
+            else:
+                await self.delete_messages(messages)
+                status, errmsg = [results.get(p, None) for p in ("status", "errmsg")]
+                if status == "error":
+                    self.log.warning(f"{name}错误: {errmsg}.")
+                    return False
+                elif status == "ok":
+                    return results
+                else:
+                    self.log.warning(f"{name}出现未知错误.")
+                    return False
             finally:
-                raise
-        except asyncio.TimeoutError:
-            await self.delete_messages(messages)
-            self.log.warning(f"{name}超时.")
-            return None
+                self.client.remove_handler(handler, group=1)
         else:
-            await self.delete_messages(messages)
-            status, errmsg = [results.get(p, None) for p in ("status", "errmsg")]
-            if status == "error":
-                self.log.warning(f"{name}错误: {errmsg}.")
-                return None
-            elif status == "ok":
-                return results
-            else:
-                self.log.warning(f"{name}出现未知错误.")
-                return None
-        finally:
-            groups[1].remove(handler)
+            return None
 
     async def _handler(
         self,
         client: Client,
         message: Message,
         cmd: str,
         future: asyncio.Future,
```

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/log.py` & `embykeeper-2.2.5/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/main.py` & `embykeeper-2.2.5/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.5/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.5/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.5/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper/telechecker/tele.py` & `embykeeper-2.2.5/embykeeper/telechecker/tele.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+from __future__ import annotations
+from collections import OrderedDict
+
 from datetime import datetime
-import time
 import asyncio
-from typing import AsyncGenerator, Optional, Union
+import inspect
+from typing import AsyncGenerator, List, Optional, Union
 
 from rich.prompt import Prompt
 from appdirs import user_data_dir
 from loguru import logger
-from pyrogram import Client as _Client
-from pyrogram import raw, types, utils, filters
+import pyrogram
+from pyrogram import raw, types, utils, filters, dispatcher
 from pyrogram.enums import SentCodeType
 from pyrogram.errors import (
     BadRequest,
     RPCError,
     Unauthorized,
     SessionPasswordNeeded,
     CodeInvalid,
     PhoneCodeInvalid,
 )
-from pyrogram.handlers import MessageHandler
+from pyrogram.handlers import MessageHandler, RawUpdateHandler
 from aiocache import Cache
 
 from .. import __name__, __version__
 from ..utils import async_partial, to_iterable
 
 logger = logger.bind(scheme="telegram")
 
@@ -37,18 +40,108 @@
         return _name(self)
 
 
 setattr(types.User, "name", property(_name))
 setattr(types.Chat, "name", property(_chat_name))
 
 
-class Client(_Client):
+class Dispatcher(dispatcher.Dispatcher):
+    def __init__(self, client: Client):
+        super().__init__(client)
+        self.mutex = asyncio.Lock()
+
+    async def start(self):
+        logger.debug("Telegram 更新分配器启动.")
+        if not self.client.no_updates:
+            self.handler_worker_tasks = [
+                self.loop.create_task(self.handler_worker()) for _ in range(self.client.workers)
+            ]
+
+    def add_handler(self, handler, group: int):
+        async def fn():
+            async with self.mutex:
+                if group not in self.groups:
+                    self.groups[group] = []
+                    self.groups = OrderedDict(sorted(self.groups.items()))
+                self.groups[group].append(handler)
+                logger.debug(f"增加了 Telegram 更新处理器: {handler.__class__.__name__}.")
+
+        self.loop.create_task(fn())
+
+    def remove_handler(self, handler, group: int):
+        async def fn():
+            async with self.mutex:
+                if group not in self.groups:
+                    raise ValueError(f"Group {group} does not exist. Handler was not removed.")
+                self.groups[group].remove(handler)
+                logger.debug(f"移除了 Telegram 更新处理器: {handler.__class__.__name__}.")
+
+        self.loop.create_task(fn())
+
+    async def handler_worker(self):
+        while True:
+            packet = await self.updates_queue.get()
+
+            if packet is None:
+                break
+
+            try:
+                update, users, chats = packet
+                parser = self.update_parsers.get(type(update), None)
+
+                parsed_update, handler_type = (
+                    await parser(update, users, chats) if parser is not None else (None, type(None))
+                )
+
+                async with self.mutex:
+                    groups = {i: g[:] for i, g in self.groups.items()}
+
+                for group in groups.values():
+                    for handler in group:
+                        args = None
+
+                        if isinstance(handler, handler_type):
+                            try:
+                                if await handler.check(self.client, parsed_update):
+                                    args = (parsed_update,)
+                            except Exception as e:
+                                logger.warning(f"Telegram Error: {e}")
+                                continue
+
+                        elif isinstance(handler, RawUpdateHandler):
+                            args = (update, users, chats)
+
+                        if args is None:
+                            continue
+
+                        try:
+                            if inspect.iscoroutinefunction(handler.callback):
+                                await handler.callback(self.client, *args)
+                            else:
+                                await self.loop.run_in_executor(
+                                    self.client.executor, handler.callback, self.client, *args
+                                )
+                        except pyrogram.StopPropagation:
+                            raise
+                        except pyrogram.ContinuePropagation:
+                            continue
+                        except Exception as e:
+                            logger.opt(exception=e).error(f"Update callback error: {e}")
+                        break
+            except pyrogram.StopPropagation:
+                pass
+            except Exception as e:
+                logger.opt(exception=e).error(f"Update handling error: {e}")
+
+
+class Client(pyrogram.Client):
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self.cache = Cache()
+        self.dispatcher = Dispatcher(self)
 
     async def authorize(self):
         if self.bot_token:
             return await self.sign_in_bot(self.bot_token)
         retry = False
         while True:
             try:
@@ -170,26 +263,22 @@
             future.set_result(message)
 
         future = asyncio.Future()
         filter = filters.chat(chat_id)
         if not outgoing:
             filter = filter & (~filters.outgoing)
         handler = MessageHandler(async_partial(handler_func, future=future), filter)
-        groups = self.dispatcher.groups
-        if 0 not in groups:
-            groups[0] = [handler]
-        else:
-            groups[0].append(handler)
+        self.add_handler(handler, group=0)
         try:
             if text:
                 await self.send_message(chat_id, text)
             msg: types.Message = await asyncio.wait_for(future, timeout)
             return msg
         finally:
-            groups[0].remove(handler)
+            self.remove_handler(handler, group=0)
 
     async def mute_chat(self, chat_id: Union[int, str], until: Union[int, datetime]):
         if isinstance(until, datetime):
             until = until.timestamp()
 
         return await self.invoke(
             raw.functions.account.UpdateNotifySettings(
```

### Comparing `embykeeper-2.2.3/embykeeper/utils.py` & `embykeeper-2.2.5/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.5/embykeeper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.3
+Version: 2.2.5
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -36,38 +36,38 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/7Q7MzwYT) 获得社区帮助.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
 
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+    - ~~EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~ (停止签到)
 - Emby 保活
 
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
 
   - 默认禁用:
@@ -98,14 +98,18 @@
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
 
+#### 其他免费 Pass
+
+您也可以通过 [Patr.cloud](https://app.patr.cloud/) ([教程](https://blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) 等平台进行部署.
+
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
@@ -412,15 +416,19 @@
 
 ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
 
 ![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
 
 ## 代码重用与开发
 
-代码架构如下:
+您可以查看 [CONTRIBUTING](https://github.com/embykeeper/embykeeper/blob/main/CONTRIBUTING.md) 以了解如何贡献代码.
+
+您也可以通过 [Discord](https://discord.gg/a4bmY38u) 参与开发讨论.
+
+项目代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
     A --> C(fa:fa-play embywatcher)
     B --checker--> E[fa:fa-robot Bot]
     B --monitor--> G[fa:fa-eye Monitor]
@@ -483,14 +491,23 @@
 请输入各群组最大获取数量 [1000]:
 ```
 
 该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
 
 另一个工具是即时信息分析:
 
+<!--
+;    用户             会话   (ChatID)                发信人   (UserID)                      信息
+; ────────────────────────────────────────────────────────────────────────────────────────────────────────────
+;   Tester  │  👥 Group A  -1001464166237   │   🤖 Bot A   1965142520   │  Welcome to the bar, what to drink?
+;   Tester  │  👥 Group A  -1001464166237   │   👤 User A  749799257    │  I want -1 cup of beer.
+;   Tester  │  👥 Group A  -1001464166237   │   👤 User B  749799257    │  A dish of asdfQwer@24dg!&*(@.
+;   Tester  │  👥 Group A  -1001464166237   │   🤖 Bot A   1965142520   │  Boom.
+-->
+
 ![follow screenshot](images/follow.svg)
 
 该工具可以实时输出消息的 ID 等信息, 以方便调试.
 
 ## 趋势
 
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.3 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.5 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -39,14 +39,15 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
+æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/7Q7MzwYT) è·å¾ç¤¾åºå¸®å©.
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
@@ -56,26 +57,26 @@
 t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
 (https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
 (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
 t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
 Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
 [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
 peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
-t.me/peach_emby_bot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https:/
-/t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Pornemby: [é¢é](https://
-t.me/pornembyservice) [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/
-PronembyTGBot2_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
-[æºå¨äºº](https://t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV)
-[ç¾¤ç»](https://t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) -
-å¶ä»é Emby ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/
-embykeeper/pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-~~BlueSea: [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/
-blueseamusic_bot)~~ (æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
-CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
-t.me/JMSIPTV_bot)~~ (æ ååº) - Emby ä¿æ´» -
+t.me/peach_emby_bot) - Pornemby: [é¢é](https://t.me/pornembyservice)
+[ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
+åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
+pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: - ~~BlueSea:
+[ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~
+(æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
+(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~
+(æ ååº) - ~~EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
+emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ (åæ­¢ç­¾å°) - Emby ä¿æ´» -
 å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
 èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
@@ -100,20 +101,22 @@
 é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
-å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». ### éè¿ Docker é¨ç½² Embykeeper
-å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://yeasy.gitbook.io/
-docker_practice/install), ç¶åæ§è¡: ```bash docker run -v $(pwd)/
-embykeeper:/app --rm -it --net=host embykeeper/embykeeper ``` å½ä»¤å°ä¼å¨
-`embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
+æ¨ä¹å¯ä»¥éè¿ [Patr.cloud](https://app.patr.cloud/) ([æç¨](https://
+blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) ç­å¹³å°è¿è¡é¨ç½². ###
+éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£
+docker](https://yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡:
+```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/
+embykeeper ``` å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml`
+æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
 (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
 "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
 `config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
 port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
 run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
@@ -249,20 +252,23 @@
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
-embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å
-ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
-telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
-Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
-``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
+embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å æ¨å¯ä»¥æ¥ç
+[CONTRIBUTING](https://github.com/embykeeper/embykeeper/blob/main/
+CONTRIBUTING.md) ä»¥äºè§£å¦ä½è´¡ç®ä»£ç . æ¨ä¹å¯ä»¥éè¿ [Discord]
+(https://discord.gg/a4bmY38u) åä¸å¼åè®¨è®º. é¡¹ç®ä»£ç æ¶æå¦ä¸:
+```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
+A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-robot Bot] B --monitor--
+> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message Messager] C --watcher--
+> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A ```
+ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
 `embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
 éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
 = 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
 "`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
 è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
@@ -278,11 +284,11 @@
 å¼åå·¥å· æ¨å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
 ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
 config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
 10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
 "åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
 è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
-å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
+å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ:  ![follow screenshot](images/follow.svg)
 è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ## è¶å¿
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
 embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.2.3/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.2.5/embykeeper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 embykeeper/__init__.py
+embykeeper/__main__.py
 embykeeper/cli.py
 embykeeper/data.py
 embykeeper/log.py
 embykeeper/settings.py
 embykeeper/utils.py
 embykeeper.egg-info/PKG-INFO
 embykeeper.egg-info/SOURCES.txt
@@ -48,14 +49,15 @@
 embykeeper/telechecker/monitor/embyhub.py
 embykeeper/telechecker/monitor/misty.py
 embykeeper/telechecker/monitor/polo.py
 embykeeper/telechecker/monitor/pornemby.py
 embykeeper/telechecker/monitor/test.py
 embykeeper/telechecker/monitor/viper.py
 embykeeperweb/__init__.py
+embykeeperweb/__main__.py
 embykeeperweb/app.py
 embykeeperweb/templates/404.html
 embykeeperweb/templates/console.html
 embykeeperweb/templates/login.html
 embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
 embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
 embykeeperweb/templates/assets/css/cascadia-code.css
```

### Comparing `embykeeper-2.2.3/embykeeperweb/app.py` & `embykeeper-2.2.5/embykeeperweb/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import time
 import signal
 
 import typer
 from loguru import logger
 from flask import Flask, render_template, request, redirect, url_for, jsonify, abort
 from flask_socketio import SocketIO
-from flask_login import LoginManager, login_user, login_required
+from flask_login import LoginManager, login_user, login_required, current_user
 
 cli = typer.Typer()
 app = Flask(__name__, static_folder="templates/assets")
 app.config["SECRET_KEY"] = os.urandom(24)
-socketio = SocketIO(app)
+socketio = SocketIO(app, cors_allowed_origins="*")
 login_manager = LoginManager()
 login_manager.init_app(app)
 login_manager.login_view = "login"
 
 app.config["args"] = None
 app.config["fd"] = None
 app.config["pid"] = None
@@ -98,40 +98,44 @@
             (pid, fd) = pty.fork()
             if pid == 0:
                 subprocess.run(["embykeeper", *app.config["args"]])
             else:
                 app.config["fd"] = fd
                 app.config["pid"] = pid
                 logger.debug(f"Embykeeper started at: {pid}.")
-            return jsonify({"status": "restarted", "pid": pid})
+            return jsonify({"status": "restarted", "pid": pid}), 201
         else:
-            return jsonify({"status": "running", "pid": app.config["pid"]})
+            return jsonify({"status": "running", "pid": app.config["pid"]}), 200
     else:
         return abort(403)
 
 
 @app.errorhandler(404)
 def page_not_found(e):
     return render_template("404.html"), 404
 
 
 @socketio.on("pty-input", namespace="/pty")
 def pty_input(data):
+    if not current_user.is_authenticated():
+        return
     if app.config["fd"]:
         os.write(app.config["fd"], data["input"].encode())
 
 
 def set_size(fd, row, col, xpix=0, ypix=0):
     logger.debug(f"Resizing pty to: {row} {col}.")
     size = struct.pack("HHHH", row, col, xpix, ypix)
     fcntl.ioctl(fd, termios.TIOCSWINSZ, size)
 
 
 @socketio.on("resize", namespace="/pty")
 def resize(data):
+    if not current_user.is_authenticated():
+        return
     if app.config["fd"]:
         set_size(app.config["fd"], data["rows"], data["cols"])
 
 
 def read_and_forward_pty_output():
     max_read_bytes = 1024 * 20
     while True:
@@ -142,14 +146,16 @@
                 output = os.read(app.config["fd"], max_read_bytes).decode(errors="ignore")
                 app.config["hist"] += output
                 socketio.emit("pty-output", {"output": output}, namespace="/pty")
 
 
 @socketio.on("embykeeper_start", namespace="/pty")
 def start(data):
+    if not current_user.is_authenticated():
+        return
     if app.config["fd"]:
         set_size(app.config["fd"], data["rows"], data["cols"])
         socketio.emit("pty-output", {"output": app.config["hist"]}, namespace="/pty")
     else:
         (pid, fd) = pty.fork()
         if pid == 0:
             subprocess.run(["embykeeper", *app.config["args"]])
@@ -159,14 +165,16 @@
             logger.debug(f"Embykeeper started at: {pid}.")
             set_size(app.config["fd"], data["rows"], data["cols"])
             socketio.start_background_task(target=read_and_forward_pty_output)
 
 
 @socketio.on("embykeeper_kill", namespace="/pty")
 def stop():
+    if not current_user.is_authenticated():
+        return
     if app.config["pid"] is not None:
         os.kill(app.config["pid"], signal.SIGINT)
         for _ in range(50):
             try:
                 os.kill(app.config["pid"], 0)
             except OSError:
                 break
```

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/404.html` & `embykeeper-2.2.5/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.2.5/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.2.5/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.2.5/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.2.5/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.2.5/embykeeperweb/templates/assets/js/console.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -26,16 +26,15 @@
     term.loadAddon(new SearchAddon.SearchAddon());
 
     term.open(document.getElementById("terminal"));
     fit.fit();
     console.debug("Web console init: ", term.cols, term.rows);
 
     const socket = io.connect("/pty", {
-        'reconnection': true,
-        'reconnectionDelay': 1000
+        'reconnection': false
     });
     socket.on("connect", () => {
         var statusIcon = document.getElementById("status-icon");
         statusIcon.style.backgroundColor = "green";
         var statusMsg = document.getElementById("status-msg");
         statusMsg.textContent = "Program Connected";
         var restartIcon = document.getElementById("restart-icon");
```

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.2.5/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/console.html` & `embykeeper-2.2.5/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/embykeeperweb/templates/login.html` & `embykeeper-2.2.5/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.3/pyproject.toml` & `embykeeper-2.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.3"
+version = "2.2.5"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-2.2.3/tests/test_cli.py` & `embykeeper-2.2.5/tests/test_cli.py`

 * *Files identical despite different names*

