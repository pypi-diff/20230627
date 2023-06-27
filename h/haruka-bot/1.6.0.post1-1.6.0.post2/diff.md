# Comparing `tmp/haruka-bot-1.6.0.post1.tar.gz` & `tmp/haruka-bot-1.6.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka-bot-1.6.0.post1.tar", last modified: Tue Jun 27 09:22:09 2023, max compression
+gzip compressed data, was "haruka-bot-1.6.0.post2.tar", last modified: Tue Jun 27 09:32:59 2023, max compression
```

## Comparing `haruka-bot-1.6.0.post1.tar` & `haruka-bot-1.6.0.post2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post1/LICENSE
--rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post1/README.md
--rw-r--r--   0        0        0      695 2023-06-27 09:08:50.665802 haruka-bot-1.6.0.post1/haruka_bot/__init__.py
--rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/__main__.py
--rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/cli/__init__.py
--rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/cli/bot.py
--rw-r--r--   0        0        0     1170 2023-06-27 09:18:39.724159 haruka-bot-1.6.0.post1/haruka_bot/cli/utils.py
--rw-r--r--   0        0        0     1390 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/config.py
--rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/database/__init__.py
--rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/database/db.py
--rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/database/models.py
--rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/libs/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/__init__.py
--rw-r--r--   0        0        0     1085 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/card.py
--rw-r--r--   0        0        0      598 2023-06-27 09:18:39.684162 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/desc.py
--rw-r--r--   0        0        0     1024 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/display.py
--rw-r--r--   0        0        0      816 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/user_profile.py
--rw-r--r--   0        0        0      456 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/at/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_off.py
--rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_on.py
--rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_agree.py
--rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_delete.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/__init__.py
--rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_off.py
--rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_on.py
--rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/help.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/live/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_off.py
--rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_on.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/__init__.py
--rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_off.py
--rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_on.py
--rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/__init__.py
--rw-r--r--   0        0        0     4710 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/dynamic_pusher.py
--rw-r--r--   0        0        0     2296 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/live_pusher.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/add_sub.py
--rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/delete_sub.py
--rw-r--r--   0        0        0     1551 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/sub_list.py
--rw-r--r--   0        0        0     8200 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/__init__.py
--rw-r--r--   0        0        0     6922 2023-06-27 09:18:54.507058 haruka-bot-1.6.0.post1/haruka_bot/utils/browser.py
--rw-r--r--   0        0        0     4887 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/captcha.py
--rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/fonts_provider.py
--rw-r--r--   0        0        0     7316 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/mobile.js
--rw-r--r--   0        0        0       97 2023-06-27 09:19:31.036443 haruka-bot-1.6.0.post1/haruka_bot/version.py
--rw-r--r--   0        0        0     1545 2023-06-27 09:03:26.103394 haruka-bot-1.6.0.post1/pyproject.toml
--rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post2/LICENSE
+-rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post2/README.md
+-rw-r--r--   0        0        0      695 2023-06-27 09:30:10.174866 haruka-bot-1.6.0.post2/haruka_bot/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/__main__.py
+-rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/cli/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/cli/bot.py
+-rw-r--r--   0        0        0     1170 2023-06-27 09:18:39.724159 haruka-bot-1.6.0.post2/haruka_bot/cli/utils.py
+-rw-r--r--   0        0        0     1390 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/config.py
+-rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/database/__init__.py
+-rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/database/db.py
+-rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/database/models.py
+-rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/libs/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/__init__.py
+-rw-r--r--   0        0        0     1085 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/card.py
+-rw-r--r--   0        0        0      598 2023-06-27 09:18:39.684162 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/desc.py
+-rw-r--r--   0        0        0     1024 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/display.py
+-rw-r--r--   0        0        0      816 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/user_profile.py
+-rw-r--r--   0        0        0      456 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/at/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_off.py
+-rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_on.py
+-rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_agree.py
+-rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_delete.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_off.py
+-rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_on.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/help.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/live/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_off.py
+-rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_off.py
+-rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_on.py
+-rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/__init__.py
+-rw-r--r--   0        0        0     4710 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/dynamic_pusher.py
+-rw-r--r--   0        0        0     2296 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/live_pusher.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/add_sub.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0        0        0     1551 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/sub_list.py
+-rw-r--r--   0        0        0     8200 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/utils/__init__.py
+-rw-r--r--   0        0        0     6922 2023-06-27 09:18:54.507058 haruka-bot-1.6.0.post2/haruka_bot/utils/browser.py
+-rw-r--r--   0        0        0     5004 2023-06-27 09:31:40.804190 haruka-bot-1.6.0.post2/haruka_bot/utils/captcha.py
+-rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     7316 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/utils/mobile.js
+-rw-r--r--   0        0        0       97 2023-06-27 09:32:29.010855 haruka-bot-1.6.0.post2/haruka_bot/version.py
+-rw-r--r--   0        0        0     1545 2023-06-27 09:03:26.103394 haruka-bot-1.6.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post2/PKG-INFO
```

### Comparing `haruka-bot-1.6.0.post1/LICENSE` & `haruka-bot-1.6.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/README.md` & `haruka-bot-1.6.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/__init__.py` & `haruka-bot-1.6.0.post2/haruka_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/cli/bot.py` & `haruka-bot-1.6.0.post2/haruka_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/cli/utils.py` & `haruka-bot-1.6.0.post2/haruka_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/config.py` & `haruka-bot-1.6.0.post2/haruka_bot/config.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/database/db.py` & `haruka-bot-1.6.0.post2/haruka_bot/database/db.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/database/models.py` & `haruka-bot-1.6.0.post2/haruka_bot/database/models.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/__init__.py` & `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/card.py` & `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/card.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/desc.py` & `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/desc.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/display.py` & `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/display.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/user_profile.py` & `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/user_profile.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_off.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_on.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_agree.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_agree.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_delete.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_delete.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_off.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_on.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/help.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/help.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_off.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_on.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_off.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_on.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/dynamic_pusher.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/dynamic_pusher.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/live_pusher.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/live_pusher.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/add_sub.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/add_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/delete_sub.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/delete_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/sub_list.py` & `haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/utils/__init__.py` & `haruka-bot-1.6.0.post2/haruka_bot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/utils/browser.py` & `haruka-bot-1.6.0.post2/haruka_bot/utils/browser.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/utils/captcha.py` & `haruka-bot-1.6.0.post2/haruka_bot/utils/captcha.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,11 +114,13 @@
                 logger.warning("[Captcha] 未检测到验证码验证结果，正在重试")
                 continue
             geetest_result = await geetest_up.text_content()
             assert geetest_result
             logger.debug(f"[Captcha] Geetest result: {geetest_result}")
             if "验证成功" in geetest_result:
                 logger.success("[Captcha] 极验网页 Tip 验证成功")
+                await page.wait_for_timeout(1000)
+                await page.wait_for_load_state("domcontentloaded")
             else:
                 logger.warning("[Captcha] 极验验证失败，正在重试")
 
     return page
```

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/utils/fonts_provider.py` & `haruka-bot-1.6.0.post2/haruka_bot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/haruka_bot/utils/mobile.js` & `haruka-bot-1.6.0.post2/haruka_bot/utils/mobile.js`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post1/pyproject.toml` & `haruka-bot-1.6.0.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bilibili",
     "bot",
 ]
-version = "1.6.0.post1"
+version = "1.6.0.post2"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/SK-415/HarukaBot"
 repository = "https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot"
```

### Comparing `haruka-bot-1.6.0.post1/PKG-INFO` & `haruka-bot-1.6.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka-bot
-Version: 1.6.0.post1
+Version: 1.6.0.post2
 Summary: Push dynamics and live informations from bilibili to QQ. Based on nonebot2.
 License: AGPL-3.0-or-later
 Keywords: nonebot,nonebot2,qqbot,bilibili,bot
 Author-email: SK-415 <2967923486@qq.com>
 Requires-Python: >=3.8,<4.0
 Project-URL: documentation, https://github.com/SK-415/HarukaBot#readme
 Project-URL: homepage, https://github.com/SK-415/HarukaBot
```

