# Comparing `tmp/aunly-bbot-1.5.0b1.tar.gz` & `tmp/aunly-bbot-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aunly-bbot-1.5.0b1.tar", last modified: Wed Jun 14 07:43:49 2023, max compression
+gzip compressed data, was "aunly-bbot-1.5.1.tar", last modified: Tue Jun 27 10:49:34 2023, max compression
```

## Comparing `aunly-bbot-1.5.0b1.tar` & `aunly-bbot-1.5.1.tar`

### file list

```diff
@@ -1,105 +1,113 @@
--rwxr-xr-x   0        0        0    34523 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/LICENSE
--rw-r--r--   0        0        0       61 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/__main__.py
--rw-r--r--   0        0        0     3361 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/bot.py
--rw-r--r--   0        0        0     1753 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/__init__.py
--rw-r--r--   0        0        0     2302 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/api.py
--rw-r--r--   0        0        0    22667 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/config.py
--rw-r--r--   0        0        0      401 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/cli/run.py
--rw-r--r--   0        0        0     1981 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/__init__.py
--rw-r--r--   0        0        0     3054 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/announcement.py
--rw-r--r--   0        0        0      944 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/bot_config.py
--rw-r--r--   0        0        0      162 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/context.py
--rw-r--r--   0        0        0     5470 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/control.py
--rw-r--r--   0        0        0    10888 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/data.py
--rw-r--r--   0        0        0     1796 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/group_config.py
--rw-r--r--   0        0        0     2620 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/log.py
--rw-r--r--   0        0        0     2957 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/core/subgroup_config.py
--rw-r--r--   0        0        0     1996 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/__init__.py
--rw-r--r--   0        0        0      322 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/add_talk.py
--rw-r--r--   0        0        0     1526 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/add.py
--rw-r--r--   0        0        0     1523 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/remove.py
--rw-r--r--   0        0        0     1088 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/announcement.py
--rw-r--r--   0        0        0     2264 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/atall.py
--rw-r--r--   0        0        0     2316 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/nick.py
--rwxr-xr-x   0        0        0    13750 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/content_resolve.py
--rw-r--r--   0        0        0     1415 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/init.py
--rw-r--r--   0        0        0     2480 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/menu/__init__.py
--rw-r--r--   0        0        0     2491 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/quit_group.py
--rw-r--r--   0        0        0     1068 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/status.py
--rw-r--r--   0        0        0     1456 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add.py
--rw-r--r--   0        0        0     2455 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add_up.py
--rw-r--r--   0        0        0     1336 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/get_subgroup.py
--rw-r--r--   0        0        0     1355 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove.py
--rw-r--r--   0        0        0     2259 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove_up.py
--rw-r--r--   0        0        0     1666 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/get_subscribe.py
--rw-r--r--   0        0        0     2547 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/subscribe.py
--rw-r--r--   0        0        0     2101 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/unsubscribe.py
--rw-r--r--   0        0        0     1447 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/add.py
--rw-r--r--   0        0        0     1446 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/remove.py
--rw-r--r--   0        0        0     3017 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/vive_dynamic.py
--rw-r--r--   0        0        0     1554 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/web_auth.py
--rw-r--r--   0        0        0     1454 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/add.py
--rw-r--r--   0        0        0     1015 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/close.py
--rw-r--r--   0        0        0     1014 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/open.py
--rw-r--r--   0        0        0     1566 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/remove.py
--rw-r--r--   0        0        0     4026 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/bot_launch.py
--rw-r--r--   0        0        0     1432 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/exception.py
--rw-r--r--   0        0        0     1940 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/invited_join_group.py
--rw-r--r--   0        0        0     1762 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/join_group.py
--rw-r--r--   0        0        0     1923 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/leave_group.py
--rw-r--r--   0        0        0     1291 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/mute.py
--rw-r--r--   0        0        0     1475 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/new_friend.py
--rw-r--r--   0        0        0      919 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/offline.py
--rw-r--r--   0        0        0     1183 2023-06-14 07:43:35.409459 aunly-bbot-1.5.0b1/aunly_bbot/function/event/prem_change.py
--rw-r--r--   0        0        0    16966 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/dynamic.py
--rw-r--r--   0        0        0    15163 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/init.py
--rw-r--r--   0        0        0    10666 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/live.py
--rw-r--r--   0        0        0     2102 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/refresh_token.py
--rw-r--r--   0        0        0      946 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/version_update.py
--rw-r--r--   0        0        0     2856 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/bcut_asr.py
--rw-r--r--   0        0        0      315 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/captcha.py
--rw-r--r--   0        0        0     7708 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/config.py
--rw-r--r--   0        0        0       93 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/exception.py
--rw-r--r--   0        0        0     1742 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/fastapi.py
--rw-r--r--   0        0        0      322 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/model/openai.py
--rw-r--r--   0        0        0     4057 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/static/bot_config.exp.yaml
--rw-r--r--   0        0        0     9159 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style.js
--rw-r--r--   0        0        0      684 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style_bak.js
--rw-r--r--   0        0        0      850 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/test.py
--rw-r--r--   0        0        0      675 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/b23_extract.py
--rw-r--r--   0        0        0     6184 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/bcut_asr.py
--rw-r--r--   0        0        0      780 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_parse.py
--rw-r--r--   0        0        0     4760 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_request.py
--rw-r--r--   0        0        0    11279 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/browser_shot.py
--rw-r--r--   0        0        0     1160 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/column_resolve.py
--rw-r--r--   0        0        0      735 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/content_summarise.py
--rw-r--r--   0        0        0     2165 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/detect_package.py
--rw-r--r--   0        0        0     8979 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/draw_bili_image.py
--rw-r--r--   0        0        0      551 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/dynamic_shot.py
--rw-r--r--   0        0        0      310 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/fastapi.py
--rw-r--r--   0        0        0     4384 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/fonts_provider.py
--rw-r--r--   0        0        0     6183 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/openai.py
--rw-r--r--   0        0        0     1103 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/pil_shot.py
--rw-r--r--   0        0        0     5069 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/send_action.py
--rw-r--r--   0        0        0     1867 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/strings.py
--rw-r--r--   0        0        0     3030 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/text2image.py
--rw-r--r--   0        0        0      516 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/time_tools.py
--rw-r--r--   0        0        0     2474 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/uid_extract.py
--rw-r--r--   0        0        0     5876 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/up_operation.py
--rw-r--r--   0        0        0     1089 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/update_version.py
--rw-r--r--   0        0        0     1666 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/verify_mah.py
--rw-r--r--   0        0        0     3803 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/video_subtitle.py
--rw-r--r--   0        0        0      713 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/utils/wordcloud.py
--rw-r--r--   0        0        0     1509 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/__init__.py
--rw-r--r--   0        0        0      415 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/__init__.py
--rw-r--r--   0        0        0     4953 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/auth.py
--rw-r--r--   0        0        0     1266 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/config.py
--rw-r--r--   0        0        0     2730 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/follow.py
--rw-r--r--   0        0        0     1664 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/home.py
--rw-r--r--   0        0        0     1459 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/user.py
--rw-r--r--   0        0        0     4009 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/ws.py
--rw-r--r--   0        0        0    87542 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/favicon.ico
--rw-r--r--   0        0        0      306 2023-06-14 07:43:35.413459 aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/index.html
--rw-r--r--   0        0        0     1720 2023-06-14 07:43:35.421459 aunly-bbot-1.5.0b1/pyproject.toml
--rw-r--r--   0        0        0     5120 2023-06-14 07:43:35.421459 aunly-bbot-1.5.0b1/readme.md
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 aunly-bbot-1.5.0b1/PKG-INFO
+-rwxr-xr-x   0        0        0    34523 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/LICENSE
+-rw-r--r--   0        0        0       61 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/__main__.py
+-rw-r--r--   0        0        0     3361 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/bot.py
+-rw-r--r--   0        0        0     1753 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/__init__.py
+-rw-r--r--   0        0        0     2302 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/api.py
+-rw-r--r--   0        0        0    23358 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/config.py
+-rw-r--r--   0        0        0      401 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/run.py
+-rw-r--r--   0        0        0     1981 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/__init__.py
+-rw-r--r--   0        0        0     3054 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/announcement.py
+-rw-r--r--   0        0        0      944 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/bot_config.py
+-rw-r--r--   0        0        0      162 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/context.py
+-rw-r--r--   0        0        0     5470 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/control.py
+-rw-r--r--   0        0        0    10888 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/data.py
+-rw-r--r--   0        0        0     1796 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/group_config.py
+-rw-r--r--   0        0        0     2620 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/log.py
+-rw-r--r--   0        0        0     2957 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/subgroup_config.py
+-rw-r--r--   0        0        0     1996 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/add_talk.py
+-rw-r--r--   0        0        0     1526 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/admin/add.py
+-rw-r--r--   0        0        0     1523 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/admin/remove.py
+-rw-r--r--   0        0        0     1088 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/announcement.py
+-rw-r--r--   0        0        0     2264 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/configure/atall.py
+-rw-r--r--   0        0        0     2316 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/configure/nick.py
+-rwxr-xr-x   0        0        0    13806 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/content_resolve.py
+-rw-r--r--   0        0        0     1415 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/init.py
+-rw-r--r--   0        0        0     2480 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/menu/__init__.py
+-rw-r--r--   0        0        0     2491 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/quit_group.py
+-rw-r--r--   0        0        0     1068 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/status.py
+-rw-r--r--   0        0        0     1456 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add.py
+-rw-r--r--   0        0        0     2455 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add_up.py
+-rw-r--r--   0        0        0     1336 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/get_subgroup.py
+-rw-r--r--   0        0        0     1355 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove.py
+-rw-r--r--   0        0        0     2259 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove_up.py
+-rw-r--r--   0        0        0     1666 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/up/get_subscribe.py
+-rw-r--r--   0        0        0     2547 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/up/subscribe.py
+-rw-r--r--   0        0        0     2101 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/up/unsubscribe.py
+-rw-r--r--   0        0        0     1447 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/vip/add.py
+-rw-r--r--   0        0        0     1446 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/vip/remove.py
+-rw-r--r--   0        0        0     3017 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/vive_dynamic.py
+-rw-r--r--   0        0        0     1554 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/web_auth.py
+-rw-r--r--   0        0        0     1454 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/add.py
+-rw-r--r--   0        0        0     1015 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/close.py
+-rw-r--r--   0        0        0     1014 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/open.py
+-rw-r--r--   0        0        0     1566 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/remove.py
+-rw-r--r--   0        0        0     4026 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/bot_launch.py
+-rw-r--r--   0        0        0     1432 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/exception.py
+-rw-r--r--   0        0        0     1940 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/invited_join_group.py
+-rw-r--r--   0        0        0     1762 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/join_group.py
+-rw-r--r--   0        0        0     1923 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/leave_group.py
+-rw-r--r--   0        0        0     1291 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/mute.py
+-rw-r--r--   0        0        0     1475 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/new_friend.py
+-rw-r--r--   0        0        0      919 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/offline.py
+-rw-r--r--   0        0        0     1183 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/prem_change.py
+-rw-r--r--   0        0        0    16966 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/pusher/dynamic.py
+-rw-r--r--   0        0        0    15163 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/pusher/init.py
+-rw-r--r--   0        0        0    10666 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/pusher/live.py
+-rw-r--r--   0        0        0     2102 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/scheduler/refresh_token.py
+-rw-r--r--   0        0        0      946 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/scheduler/version_update.py
+-rw-r--r--   0        0        0     2856 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/bcut_asr.py
+-rw-r--r--   0        0        0      315 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/captcha.py
+-rw-r--r--   0        0        0     8284 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/config.py
+-rw-r--r--   0        0        0       93 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/exception.py
+-rw-r--r--   0        0        0     1742 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/fastapi.py
+-rw-r--r--   0        0        0      322 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/openai.py
+-rw-r--r--   0        0        0     4174 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/bot_config.exp.yaml
+-rw-r--r--   0        0        0     9159 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/mobile_style.js
+-rw-r--r--   0        0        0      684 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/mobile_style_bak.js
+-rw-r--r--   0        0        0     1187 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7534 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     2098 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/openai.png
+-rw-r--r--   0        0        0      850 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/test.py
+-rw-r--r--   0        0        0      675 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/b23_extract.py
+-rw-r--r--   0        0        0     6220 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/bcut_asr.py
+-rw-r--r--   0        0        0      780 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_parse.py
+-rw-r--r--   0        0        0     4760 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_request.py
+-rw-r--r--   0        0        0    11463 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/browser_shot.py
+-rw-r--r--   0        0        0     1160 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/column_resolve.py
+-rw-r--r--   0        0        0      735 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/content_summarise.py
+-rw-r--r--   0        0        0     2165 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/detect_package.py
+-rw-r--r--   0        0        0    16749 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/draw_bili_image.py
+-rw-r--r--   0        0        0      551 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/dynamic_shot.py
+-rw-r--r--   0        0        0      310 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/fastapi.py
+-rw-r--r--   0        0        0     4384 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     6183 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/openai.py
+-rw-r--r--   0        0        0     1103 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/pil_shot.py
+-rw-r--r--   0        0        0     5069 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/send_action.py
+-rw-r--r--   0        0        0     1867 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/strings.py
+-rw-r--r--   0        0        0     3545 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/text2image.py
+-rw-r--r--   0        0        0      516 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/time_tools.py
+-rw-r--r--   0        0        0     2474 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/uid_extract.py
+-rw-r--r--   0        0        0     5876 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/up_operation.py
+-rw-r--r--   0        0        0     1089 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/update_version.py
+-rw-r--r--   0        0        0     1666 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/verify_mah.py
+-rw-r--r--   0        0        0     3803 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/video_subtitle.py
+-rw-r--r--   0        0        0      713 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/wordcloud.py
+-rw-r--r--   0        0        0     1509 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/__init__.py
+-rw-r--r--   0        0        0     4953 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/auth.py
+-rw-r--r--   0        0        0     1266 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/config.py
+-rw-r--r--   0        0        0     2730 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/follow.py
+-rw-r--r--   0        0        0     1664 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/home.py
+-rw-r--r--   0        0        0     1459 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/user.py
+-rw-r--r--   0        0        0     4009 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/ws.py
+-rw-r--r--   0        0        0    87542 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/static/html/favicon.ico
+-rw-r--r--   0        0        0      306 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/static/html/index.html
+-rw-r--r--   0        0        0     1735 2023-06-27 10:49:17.121931 aunly-bbot-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5120 2023-06-27 10:49:17.121931 aunly-bbot-1.5.1/readme.md
+-rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.5.1/PKG-INFO
```

### Comparing `aunly-bbot-1.5.0b1/LICENSE` & `aunly-bbot-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/bot.py` & `aunly-bbot-1.5.1/aunly_bbot/bot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/cli/__init__.py` & `aunly-bbot-1.5.1/aunly_bbot/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/cli/api.py` & `aunly-bbot-1.5.1/aunly_bbot/cli/api.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/cli/config.py` & `aunly-bbot-1.5.1/aunly_bbot/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
                 [Choice("是（开启）"), Choice("否（关闭）")],
                 allow_filter=False,
                 default_select=1,
                 annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
             ).prompt()
             self.config["Bilibili"]["use_browser"] = browser.name == "是（开启）"
             self.bilibili_mobile_style()
+            self.render_style()
             self.allow_fallback()
         else:
             self.config["Bilibili"]["use_browser"] = False
 
     def bilibili_mobile_style(self):
         if is_full:
             mobile_style = ListPrompt(
@@ -247,14 +248,26 @@
                 allow_filter=False,
                 annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
             ).prompt()
             self.config["Bilibili"]["mobile_style"] = mobile_style.name == "是（开启）"
         else:
             self.config["Bilibili"]["mobile_style"] = False
 
+    def render_style(self):
+        if is_full:
+            mobile_style = ListPrompt(
+                "请选择使用的视频信息渲染模板？（bbot_default无需浏览器，其他均需求浏览器）",
+                [Choice("bbot_default"), Choice("style_blue")],
+                allow_filter=False,
+                annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
+            ).prompt()
+            self.config["Bilibili"]["render_style"] = mobile_style.name
+        else:
+            self.config["Bilibili"]["render_style"] = "bbot_default"
+
     def allow_fallback(self):
         allow_fallback = ListPrompt(
             "是否允许使用备用动态图片渲染（在浏览器截图失败时尝试使用）？",
             [Choice("是（开启）"), Choice("否（关闭）")],
             allow_filter=False,
             annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
         ).prompt()
@@ -284,15 +297,19 @@
         else:
             click.secho("输入的 OpenAI Token 不合法（应以 sk- 开头）", fg="bright_red", bold=True)
             self.openai_api_token()
 
     def openai_model(self):
         openai_model = ListPrompt(
             "请选择 OpenAI 模型",
-            [Choice("gpt-3.5-turbo-0613"), Choice("gpt-3.5-turbo-16k-0613"), Choice("gpt-4-0613")],
+            [
+                Choice("gpt-3.5-turbo-0613"),
+                Choice("gpt-3.5-turbo-16k-0613"),
+                Choice("gpt-4-0613"),
+            ],
             allow_filter=False,
             annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
         ).prompt()
         self.config["Bilibili"]["openai_model"] = openai_model.name
 
     def openai_proxy(self):
         if openai_proxy_url := InputPrompt("请输入 OpenAI 代理地址（留空则不使用代理）: ").prompt():
@@ -304,18 +321,19 @@
                 self.openai_proxy()
             self.config["Bilibili"]["openai_proxy"] = openai_proxy_url
 
     def bilibili_username(self):
         username = InputPrompt("请输入 Bilibili 用户名: （可用于 AI 总结时获取 Bilibili 的 AI 字幕）").prompt()
         if not username or username == "":
             self.config["Bilibili"]["username"] = username
-            return click.secho("用户名为空，已关闭对应功能！", fg="bright_red", bold=True)
+            click.secho("用户名为空，已关闭对应功能！", fg="bright_red", bold=True)
+            return 
         elif not username.isdigit():
             click.secho("用户名不合法！", fg="bright_red", bold=True)
-            self.bilibili_username()
+            return self.bilibili_username()
         self.config["Bilibili"]["username"] = username
         self.bilibili_password()
 
     def bilibili_password(self):
         password = InputPrompt("请输入 Bilibili 密码: ", is_password=True).prompt()
         if not password:
             click.secho("密码不能为空！", fg="bright_red", bold=True)
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/__init__.py` & `aunly-bbot-1.5.1/aunly_bbot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/announcement.py` & `aunly-bbot-1.5.1/aunly_bbot/core/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/bot_config.py` & `aunly-bbot-1.5.1/aunly_bbot/core/bot_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/control.py` & `aunly-bbot-1.5.1/aunly_bbot/core/control.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/data.py` & `aunly-bbot-1.5.1/aunly_bbot/core/data.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/group_config.py` & `aunly-bbot-1.5.1/aunly_bbot/core/group_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/log.py` & `aunly-bbot-1.5.1/aunly_bbot/core/log.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/core/subgroup_config.py` & `aunly-bbot-1.5.1/aunly_bbot/core/subgroup_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/__init__.py` & `aunly-bbot-1.5.1/aunly_bbot/function/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/add.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/admin/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/admin/remove.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/admin/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/announcement.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/atall.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/configure/atall.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/configure/nick.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/configure/nick.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/content_resolve.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/content_resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ...core.bot_config import BotConfig
 from ...model.exception import AbortError
 from ...utils.column_resolve import get_cv
 from ...core.data import ContentResolveData
 from ...core.control import Interval, Permission
 from ...utils.video_subtitle import get_subtitle
 from ...utils.bilibili_parse import extract_bilibili_info
-from ...utils.draw_bili_image import binfo_image_create
+from ...utils.draw_bili_image import BiliVideoImage
 from ...utils.text2image import rich_text2image, browser_text2image
 from ...utils.bilibili_request import get_b23_url, grpc_get_view_info
 from ...utils.content_summarise import column_summarise, subtitle_summarise
 
 channel = Channel.current()
 
 
@@ -47,15 +47,16 @@
 
         archive_data = ContentResolveData(aid=aid)
         archive_data.title = title
         await Interval.manual(aid + group.id, 30)
         try:
             logger.info(f"开始生成视频信息图片：{aid}")
             b23_url = await get_b23_url(f"https://www.bilibili.com/video/{bvid}")
-            image = await binfo_image_create(video_info, b23_url)
+
+            image = await (await BiliVideoImage.from_view_rely(video_info, b23_url)).render(BotConfig.Bilibili.render_style)
             info_message = await app.send_group_message(
                 group,
                 MessageChain(
                     Image(data_bytes=image),
                     f"\n{b23_url}",
                 ),
                 quote=source,
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/init.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/menu/__init__.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/quit_group.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/quit_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/status.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/status.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/add_up.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/get_subgroup.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/get_subgroup.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/subgroup/remove_up.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/get_subscribe.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/up/get_subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/subscribe.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/up/subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/up/unsubscribe.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/up/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/add.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/vip/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vip/remove.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/vip/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/vive_dynamic.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/vive_dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/web_auth.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/web_auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/add.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/close.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/close.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/open.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/open.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/command/whitelist/remove.py` & `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/bot_launch.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/bot_launch.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/exception.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/exception.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/invited_join_group.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/invited_join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/join_group.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/leave_group.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/leave_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/mute.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/mute.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/new_friend.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/new_friend.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/offline.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/offline.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/event/prem_change.py` & `aunly-bbot-1.5.1/aunly_bbot/function/event/prem_change.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/dynamic.py` & `aunly-bbot-1.5.1/aunly_bbot/function/pusher/dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/init.py` & `aunly-bbot-1.5.1/aunly_bbot/function/pusher/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/pusher/live.py` & `aunly-bbot-1.5.1/aunly_bbot/function/pusher/live.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/refresh_token.py` & `aunly-bbot-1.5.1/aunly_bbot/function/scheduler/refresh_token.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/function/scheduler/version_update.py` & `aunly-bbot-1.5.1/aunly_bbot/function/scheduler/version_update.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/model/bcut_asr.py` & `aunly-bbot-1.5.1/aunly_bbot/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/model/config.py` & `aunly-bbot-1.5.1/aunly_bbot/model/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,28 +48,31 @@
 class _Bilibili(BaseModel, extra=Extra.ignore):
     username: Optional[str]
     password: Optional[str]
     use_login: bool = False
     use_browser: bool = True
     allow_fallback: bool = True
     mobile_style: bool = True
+    render_style: Literal["bbot_default", "style_blue"] = "bbot_default"
     concurrency: int = 5
     dynamic_font: str = "HarmonyOS_Sans_SC_Medium.ttf"
     dynamic_font_source: Literal["local", "remote"] = "local"
     openai_summarization: bool = False
     openai_api_token: Optional[str] = None
     openai_model: str = "gpt-3.5-turbo-0301"
     openai_proxy: Optional[AnyHttpUrl] = None
     openai_cooldown: int = 60
     openai_whitelist_users: Optional[list[int]] = None
     openai_promot_version: int = 2
     use_wordcloud: bool = False
     use_bcut_asr: bool = False
     asr_length_threshold: int = 60
-    captcha_address: Optional[AnyHttpUrl] = None
+    captcha_address: Optional[AnyHttpUrl] = AnyHttpUrl(
+        "https://captcha-cd.ngworks.cn", scheme="https"
+    )
 
     # 验证是否可以登录
     @validator("use_login", always=True)
     def can_use_login(cls, use_login, values):
         if not use_login:
             return use_login
         click.secho("已检测到开启 BiliBili 登录模式，不推荐使用", fg="bright_yellow", bold=True)
@@ -123,14 +126,26 @@
             return 50
         elif concurrency < 1:
             click.secho("gRPC 并发数小于 1，已自动调整为 1", fg="bright_yellow")
             return 1
         else:
             return concurrency
 
+    @validator("render_style")
+    def can_use_style(cls, render_style):
+        if render_style == "bbot_default":
+            return render_style
+        try:
+            import playwright  # noqa  # type: ignore
+
+            return render_style
+        except ImportError:
+            click.secho("未安装 playwright，如需使用非默认的渲染样式，请安装 graiax-playwright", fg="bright_red")
+            sys.exit()
+
 
 class _Event(BaseModel, extra=Extra.ignore):
     mute: bool = True
     permchange: bool = True
     push: bool = True
     subscribe: bool = True
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/model/fastapi.py` & `aunly-bbot-1.5.1/aunly_bbot/model/fastapi.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/static/bot_config.exp.yaml` & `aunly-bbot-1.5.1/aunly_bbot/static/bot_config.exp.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -15,26 +15,27 @@
   use_login: false                        # 是否使用登录的 BiliBili 账号进行动态监听（没事不建议开）
   use_browser: true                       # 是否使用浏览器进行动态截图
   allow_fallback: true                    # 是否允许使用截图失败后的备用方案（PIL）渲染动态
   username:                               # BiliBili 账号，若填写则会在启动后自动登录，并且用于部分功能，如 AI 字幕
   password:                               # BiliBili 密码
   concurrency: 5                          # 未登录时发送 gRPC 请求的并发数量(1 ~ 50)
   dynamic_font: "HarmonyOS_Sans_SC_Medium.ttf" # 自定义动态字体
+  render_style: "bbot_default"            # 自定义渲染样式，可选值: "bbot_default", "style_blue"
   dynamic_font_source: "local"            # 自定义动态字体来源, 可选值: "local", "remote", 为 "local" 时请将字体文件放在 data/font 目录下
   openai_summarization: false             # 是否使用 OpenAI 进行视频和专栏的 AI 总结
   openai_api_token: "sk-xxxxxxxxxxxxxx"   # OpenAI API Token
   openai_model: "gpt-3.5-turbo-0301"      # OpenAI 模型
   openai_proxy: "http://localhost:7890"   # 请求 OpenAI 所用的代理
   openai_cooldown: 60                     # OpenAI 调用冷却时间（秒）
   openai_whitelist_users: []              # OpenAI 调用冷却白名单用户（即使在冷却时间内也可以调用）
   openai_promot_version: 2                # OpenAI 提示词版本，当前可选值: 1, 2
   use_wordcloud: true                     # 是否使用词云
   use_bcut_asr: true                      # 是否使用 BCut 接口进行 AI 语音识别
   asr_length_threshold: 60                # 调用语音识别的最小长度阈值（秒）
-  captcha_address: null                   # 验证码识别服务地址
+  captcha_address: "https://captcha-cd.ngworks.cn" # 验证码识别服务地址
 Event:
   mute: true                              # 是否向管理员发送被禁言的事件提醒。
   permchange: true                        # 是否向管理员发送权限变更的事件提醒。
   push: true                              # 是否向管理员发送推送的事件提醒。
   subscribe: true                         # 是否向管理员发送订阅的事件提醒。
 Webui:
   webui_host: "0.0.0.0"                   # WebUI 监听地址
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style.js` & `aunly-bbot-1.5.1/aunly_bbot/static/mobile_style.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/static/mobile_style_bak.js` & `aunly-bbot-1.5.1/aunly_bbot/static/mobile_style_bak.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/test.py` & `aunly-bbot-1.5.1/aunly_bbot/test.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/b23_extract.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/b23_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/bcut_asr.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/bcut_asr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import time
-import httpx
+from __future__ import annotations
 
+import time
 from os import PathLike
 from pathlib import Path
-from loguru import logger
 from typing import Literal, Optional
 
+import httpx
+from loguru import logger
+
 from ..model.bcut_asr import (
+    ResourceCompleteRspSchema,
+    ResourceCreateRspSchema,
     ResultRspSchema,
     TaskCreateRspSchema,
-    ResourceCreateRspSchema,
-    ResourceCompleteRspSchema,
 )
 
 __version__ = "0.0.2"
 
 API_REQ_UPLOAD = "https://member.bilibili.com/x/bcut/rubick-interface/resource/create"  # 申请上传
 API_COMMIT_UPLOAD = (
     "https://member.bilibili.com/x/bcut/rubick-interface/resource/create/complete"  # 提交上传
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_parse.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_parse.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/bilibili_request.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/browser_shot.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/browser_shot.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from ..model.captcha import CaptchaResponse
 
 from .fonts_provider import get_font
 
 
 error_path = Path("data").joinpath("error")
 error_path.mkdir(parents=True, exist_ok=True)
+captcha_path = Path("data").joinpath("captcha")
+captcha_path.mkdir(parents=True, exist_ok=True)
 mobile_style_js = Path(__file__).parent.parent.joinpath("static", "mobile_style.js")
 font_mime_map = {
     "collection": "font/collection",
     "otf": "font/otf",
     "sfnt": "font/sfnt",
     "ttf": "font/ttf",
     "woff": "font/woff",
@@ -184,15 +186,15 @@
             else None,
         )
 
     with contextlib.suppress(TimeoutError):
         await page.goto(url, wait_until="networkidle", timeout=20000)
 
     if captcha_address:
-        captcha_baseurl = f"{captcha_address.scheme}://{captcha_address.host}:{captcha_address.port}/captcha/select"
+        captcha_baseurl = f"{captcha_address}/captcha/select"
         while captcha_image_body or captcha_result is False:
             logger.warning("[Captcha] 需要人机验证，正在尝试自动解决验证码")
             captcha_image = await page.query_selector(".geetest_item_img")
             assert captcha_image
             captcha_size = await captcha_image.bounding_box()
             assert captcha_size
             origin_image_size = 344, 384
@@ -217,15 +219,15 @@
                         "y": point[1] * captcha_size["height"] / origin_image_size[1],
                     }
                     await captcha_image.click(position=Position(**real_click_points))
                     await page.wait_for_timeout(800)
                 captcha_image_body = ""
                 await page.click("text=确认")
                 geetest_up = await page.wait_for_selector(".geetest_up", state="visible")
-                Path("captcha.jpg").write_bytes(await page.screenshot())
+                await page.screenshot(path=captcha_path.joinpath(f"{last_captcha_id}.jpg"))
                 if not geetest_up:
                     logger.warning("[Captcha] 未检测到验证码验证结果，正在重试")
                     continue
                 geetest_result = await geetest_up.text_content()
                 assert geetest_result
                 logger.debug(f"[Captcha] Geetest result: {geetest_result}")
                 if "验证成功" in geetest_result:
@@ -237,15 +239,18 @@
                     await page.wait_for_load_state(state="domcontentloaded", timeout=20000)
 
     if "bilibili.com/404" in page.url:
         logger.warning(f"[Bilibili推送] {dynid} 动态不存在")
         raise Notfound
 
     await page.wait_for_load_state(state="domcontentloaded", timeout=20000)
-    await page.wait_for_selector(".opus-module-author", state="visible")
+    if "opus" in page.url:
+        await page.wait_for_selector(".opus-module-author", state="visible")
+    else:
+        await page.wait_for_selector(".dyn-header__author__face", state="visible")
 
     await page.add_script_tag(path=mobile_style_js)
     await page.wait_for_function("getMobileStyle()")
 
     await page.evaluate(
         f"setFont('{BotConfig.Bilibili.dynamic_font}', '{BotConfig.Bilibili.dynamic_font_source}')"
     )
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/column_resolve.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/column_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/content_summarise.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/content_summarise.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/detect_package.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/detect_package.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/dynamic_shot.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/dynamic_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/fonts_provider.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/openai.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/openai.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/pil_shot.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/pil_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/send_action.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/send_action.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/strings.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/strings.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/text2image.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/text2image.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
-
+import re
 from io import BytesIO
 from pathlib import Path
+
 from graia.ariadne.app import Ariadne
-from PIL import Image, ImageFont, ImageDraw
+from PIL import Image, ImageDraw, ImageFont
 
-from .strings import get_cut_str
 from .fonts_provider import get_font_sync
-
+from .strings import get_cut_str
 
 data_path = Path("data", "render")
 data_path.mkdir(parents=True, exist_ok=True)
 font = ImageFont.truetype(str(get_font_sync("sarasa-mono-sc-semibold.ttf")), size=20)
 
 
 async def text2image(text: str, cut=64) -> bytes:
@@ -33,17 +33,18 @@
         qtables="web_high",
     )
     return imageio.getvalue()
 
 
 async def rich_text2image(data: str):
     from io import BytesIO
+
+    from dynamicadaptor.Content import RichTextDetail, Text
     from minidynamicrender.DynConfig import ConfigInit
     from minidynamicrender.DynText import DynTextRender
-    from dynamicadaptor.Content import Text, RichTextDetail
 
     from .fonts_provider import get_font
 
     config = ConfigInit(
         data_path=str(data_path),
         font_path={
             "text": str(await get_font("HarmonyOS_Sans_SC_Medium.ttf")),
@@ -69,22 +70,44 @@
         if image:
             bio = BytesIO()
             image.convert("RGB").save(bio, "jpeg", optimize=True)
             return bio.getvalue()
 
 
 async def browser_text2image(data: str):
-    from graiax.text2img.playwright import convert_md
+    import jinja2
     from graiax.playwright.interface import PlaywrightContext
-    from graiax.text2img.playwright.renderer import BuiltinCSS
+
+    from .browser_shot import fill_font
 
     app = Ariadne.current()
     browser_context = app.launch_manager.get_interface(PlaywrightContext).context
-    page = await browser_context.new_page()
-    await page.set_viewport_size({"width": 400, "height": 100})
-    md = convert_md(data)
-    css = "\n".join(BuiltinCSS.github.value)
-    await page.set_content(
-        '<html><head><meta name="viewport" content="width=device-width,initial-scale=1.0">'
-        f"<style>{css}</style></head><body>{md}<body></html>"
+
+    src = "openai"
+    data = r"\n".join(data.splitlines())
+
+    summary = Path(__file__).parent.parent.joinpath("static", "summary")
+    template_env = jinja2.Environment(
+        loader=jinja2.FileSystemLoader(summary),
+        enable_async=True,
+    )
+    template_path = f"file:///{summary.joinpath('index.html').absolute()}".replace(
+        "////", "///"
     )
-    return await page.screenshot(full_page=True, type="jpeg", quality=95)
+    template = template_env.get_template("index.html")
+    html = await template.render_async(
+        **{
+            "data": data,
+            "src": src,
+        }
+    )
+
+    async with await browser_context.new_page() as page:
+        await page.route(re.compile("^https://fonts.bbot/(.+)$"), fill_font)
+        await page.set_viewport_size({"width": 800, "height": 2000})
+        await page.goto(template_path)
+        await page.set_content(html, wait_until="networkidle")
+        await page.wait_for_timeout(5)
+        img_raw = await page.get_by_alt_text("main").screenshot(
+            type="png",
+        )
+    return img_raw
```

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/time_tools.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/uid_extract.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/uid_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/up_operation.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/up_operation.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/update_version.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/update_version.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/verify_mah.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/verify_mah.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/video_subtitle.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/utils/wordcloud.py` & `aunly-bbot-1.5.1/aunly_bbot/utils/wordcloud.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/__init__.py` & `aunly-bbot-1.5.1/aunly_bbot/website/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/auth.py` & `aunly-bbot-1.5.1/aunly_bbot/website/api/router/auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/config.py` & `aunly-bbot-1.5.1/aunly_bbot/website/api/router/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/follow.py` & `aunly-bbot-1.5.1/aunly_bbot/website/api/router/follow.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/home.py` & `aunly-bbot-1.5.1/aunly_bbot/website/api/router/home.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/user.py` & `aunly-bbot-1.5.1/aunly_bbot/website/api/router/user.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/api/router/ws.py` & `aunly-bbot-1.5.1/aunly_bbot/website/api/router/ws.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/aunly_bbot/website/static/html/favicon.ico` & `aunly-bbot-1.5.1/aunly_bbot/website/static/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/pyproject.toml` & `aunly-bbot-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aunly-bbot"
-version = "1.5.0-beta1"
+version = "1.5.1"
 description = "一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人"
 readme = "readme.md"
 keywords = [
     "graia",
     "graiax",
     "bilibili",
     "qqbot",
@@ -51,14 +51,15 @@
 [project.optional-dependencies]
 full = [
     "graiax-playwright>=0.2.4",
     "graiax-text2img-playwright>=0.4.0",
     "wordcloud>=1.9.2",
     "jieba>=0.42.1",
     "edgegpt>=0.10.13",
+    "jinja2>=3.1.2",
 ]
 
 [project.scripts]
 bbot = "aunly_bbot.__main__:main"
 
 [tool.pdm.build]
 includes = [
```

### Comparing `aunly-bbot-1.5.0b1/readme.md` & `aunly-bbot-1.5.1/readme.md`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.0b1/PKG-INFO` & `aunly-bbot-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aunly-bbot
-Version: 1.5.0-beta1
+Version: 1.5.1
 Summary: 一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人
 License: AGPL3.0
 Keywords: graia,graiax,bilibili,qqbot,grpc,playwright,fastapi,bot,openai,chatgpt
 Author-email: djkcyl <cyl@cyllive.cn>
 Requires-Python: >=3.9,<4.0
 Provides-Extra: full
 Project-URL: documentation, https://github.com/djkcyl/BBot-Graia/blob/master/readme.md
```

