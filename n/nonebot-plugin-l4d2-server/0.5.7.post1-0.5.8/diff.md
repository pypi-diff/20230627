# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.7.post1.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.7.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.8.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.7.post1.tar` & `nonebot_plugin_l4d2_server-0.5.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-25 13:39:28.959299 nonebot_plugin_l4d2_server-0.5.7.post1/LICENSE
--rw-r--r--   0        0        0     5683 2023-06-25 13:39:28.959299 nonebot_plugin_l4d2_server-0.5.7.post1/README.md
--rw-r--r--   0        0        0    19815 2023-06-25 13:39:28.963299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-25 13:39:28.963299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1714 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1879 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3736 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10990 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8989 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5960 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     9672 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    15320 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1610 2023-06-25 13:39:28.975299 nonebot_plugin_l4d2_server-0.5.7.post1/pyproject.toml
--rw-r--r--   0        0        0     7553 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.7.post1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-27 14:50:54.855206 nonebot_plugin_l4d2_server-0.5.8/LICENSE
+-rw-r--r--   0        0        0     5683 2023-06-27 14:50:54.855206 nonebot_plugin_l4d2_server-0.5.8/README.md
+-rw-r--r--   0        0        0    19839 2023-06-27 14:50:54.859206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-27 14:50:54.859206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-27 14:50:54.859206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1714 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1879 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3736 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10952 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8989 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5960 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     9675 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    15320 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1604 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.8/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/LICENSE` & `nonebot_plugin_l4d2_server-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/README.md` & `nonebot_plugin_l4d2_server-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 require('nonebot_plugin_apscheduler')
 require('nonebot_plugin_htmlrender')
 require('nonebot_plugin_txt2img')
 from .l4d2_web import web,webUI
 
 from typing import Tuple,Union,List
 from time import sleep
+import time
 
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg
 from nonebot import get_driver, require
 from typing import Annotated
 from nonebot.params import Keyword
@@ -282,25 +283,26 @@
         now_path = l4_config.l4_ipall[l4_config.l4_number]['location']
         await matcher.send(f'当前的路径为\n{str(l4_config.l4_number+1)}、{now_path}')
         
         
 @queries_comm.handle()
 async def _(matcher:Matcher,event:MessageEvent,keyword:str = Keyword()):
     msg = event.get_plaintext()
+ 
     if not msg:
         await matcher.finish('ip格式如中括号内【127.0.0.1】【114.51.49.19:1810】')
     ip = msg.split(keyword)[-1].split('\r')[0].split('\n')[0].split(' ')
     for one_msg in ip:
         if one_msg and one_msg[-1].isdigit():
             break
     if not one_msg:
         await matcher.finish()
     ip_list = split_maohao(one_msg)
     msg = await queries_server(ip_list)
-    await str_to_picstr(msg,matcher)
+    await str_to_picstr(msg,matcher,keyword)
     
 
 @add_queries.handle()
 async def _(matcher:Matcher,event:GroupMessageEvent,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if len(msg)==0:
         await matcher.finish('请在该指令后加入参数，例如【114.51.49.19:1810】')
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     message += '地图：' + mse['map_'] + '\n'
     message += f"玩家：{mse['players']} / {mse['max_players']}\n"
     print(mse['Players'])
     try:
         message += await msg_ip_to_list(mse['Players'])
     except (KeyError):
         message += '服务器里，是空空的呢\n'
-    message += 'connect ' + mse['ip']
     return message
 
 
 
 async def get_server_ip(number):
     group,host,port = await si.query_number(number)
     try:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,14 @@
     """查询ip返回信息"""
     ip = msg[0]
     port = msg[1]
     msgs = ''
     try:
         msgs = await  queries(ip,port)
         msgs += await player_queries(ip,port)
-        msgs += f"connect {ip}:{port}"
     except (struct.error,TimeoutError):
         pass
     # except Exception:
         # msgs = '有无法识别的用户名'
         # return msgs
     return msgs
 
@@ -305,23 +304,23 @@
     for i in range(len(msg) - 1, -1, -1):
         if msg[i].isdigit():
             last_digit = msg[i]
             new_msg = msg[:i]
             return new_msg, last_digit
     return msg, ''
 
-async def str_to_picstr(push_msg:str,matcher:Matcher):
+async def str_to_picstr(push_msg:str,matcher:Matcher,keyword:str = None):
     """判断图片输出还是正常输出"""
     if l4_config.l4_image:
         lines = push_msg.splitlines()
         first_str = lines[0]
         last_str = lines[-1]
         push_msg = '\n'.join(lines[1:-1])
         if l4_config.l4_connect:
             await matcher.send(mode_txt_to_img(first_str,push_msg)+last_str)
         else:
             await matcher.send(mode_txt_to_img(first_str,push_msg))
     else:
-        if l4_config.l4_connect:
+        if l4_config.l4_connect or keyword== "connect":
             await matcher.send(push_msg)
         else:
-            await matcher.send('\n'.join(push_msg.splitlines()[1:-1]))
+            await matcher.send('\n'.join(push_msg.splitlines()[1:-2]))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.7.post1"
+version = "0.5.8"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7.post1/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.7.post1
+Version: 0.5.8
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.7.post1
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.8 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

