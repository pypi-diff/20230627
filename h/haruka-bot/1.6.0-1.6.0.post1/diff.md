# Comparing `tmp/haruka-bot-1.6.0.tar.gz` & `tmp/haruka-bot-1.6.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka-bot-1.6.0.tar", last modified: Tue Jun 27 08:51:15 2023, max compression
+gzip compressed data, was "haruka-bot-1.6.0.post1.tar", last modified: Tue Jun 27 09:22:09 2023, max compression
```

## Comparing `haruka-bot-1.6.0.tar` & `haruka-bot-1.6.0.post1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    34522 2023-06-27 08:46:55.526760 haruka-bot-1.6.0/LICENSE
--rw-r--r--   0        0        0     2790 2023-06-27 08:46:55.526760 haruka-bot-1.6.0/README.md
--rw-r--r--   0        0        0      253 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/__init__.py
--rw-r--r--   0        0        0       61 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/__main__.py
--rw-r--r--   0        0        0      189 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/cli/__init__.py
--rw-r--r--   0        0        0      734 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/cli/bot.py
--rw-r--r--   0        0        0     1169 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/cli/utils.py
--rw-r--r--   0        0        0     1390 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/config.py
--rw-r--r--   0        0        0       49 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/database/__init__.py
--rw-r--r--   0        0        0    10155 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/database/db.py
--rw-r--r--   0        0        0     1936 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/database/models.py
--rw-r--r--   0        0        0       30 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/__init__.py
--rw-r--r--   0        0        0     1464 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/card.py
--rw-r--r--   0        0        0      597 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/desc.py
--rw-r--r--   0        0        0     1023 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/display.py
--rw-r--r--   0        0        0      810 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/user_profile.py
--rw-r--r--   0        0        0      456 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 08:47:26.570760 haruka-bot-1.6.0/haruka_bot/plugins/at/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/at/at_off.py
--rw-r--r--   0        0        0     1421 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/at/at_on.py
--rw-r--r--   0        0        0      678 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/auto_agree.py
--rw-r--r--   0        0        0      875 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/auto_delete.py
--rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/dynamic/__init__.py
--rw-r--r--   0        0        0     1048 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_off.py
--rw-r--r--   0        0        0     1039 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_on.py
--rw-r--r--   0        0        0      734 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/help.py
--rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/live/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/live/live_off.py
--rw-r--r--   0        0        0     1012 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/live/live_on.py
--rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/permission/__init__.py
--rw-r--r--   0        0        0     1180 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_off.py
--rw-r--r--   0        0        0     1201 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_on.py
--rw-r--r--   0        0        0       58 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/pusher/__init__.py
--rw-r--r--   0        0        0     4710 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/pusher/dynamic_pusher.py
--rw-r--r--   0        0        0     2296 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/pusher/live_pusher.py
--rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/sub/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/sub/add_sub.py
--rw-r--r--   0        0        0     1021 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/sub/delete_sub.py
--rw-r--r--   0        0        0     1551 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/sub/sub_list.py
--rw-r--r--   0        0        0     8200 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/__init__.py
--rw-r--r--   0        0        0     6921 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/browser.py
--rw-r--r--   0        0        0     4887 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/captcha.py
--rw-r--r--   0        0        0      702 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/fonts_provider.py
--rw-r--r--   0        0        0     7316 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/mobile.js
--rw-r--r--   0        0        0       92 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/version.py
--rw-r--r--   0        0        0     1560 2023-06-27 08:46:55.566760 haruka-bot-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 haruka-bot-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post1/LICENSE
+-rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post1/README.md
+-rw-r--r--   0        0        0      695 2023-06-27 09:08:50.665802 haruka-bot-1.6.0.post1/haruka_bot/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/__main__.py
+-rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/cli/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/cli/bot.py
+-rw-r--r--   0        0        0     1170 2023-06-27 09:18:39.724159 haruka-bot-1.6.0.post1/haruka_bot/cli/utils.py
+-rw-r--r--   0        0        0     1390 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/config.py
+-rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/database/__init__.py
+-rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/database/db.py
+-rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/database/models.py
+-rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/libs/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/__init__.py
+-rw-r--r--   0        0        0     1085 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/card.py
+-rw-r--r--   0        0        0      598 2023-06-27 09:18:39.684162 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/desc.py
+-rw-r--r--   0        0        0     1024 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/display.py
+-rw-r--r--   0        0        0      816 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/user_profile.py
+-rw-r--r--   0        0        0      456 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/at/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_off.py
+-rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_on.py
+-rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_agree.py
+-rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_delete.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_off.py
+-rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_on.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/help.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/live/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_off.py
+-rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_off.py
+-rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_on.py
+-rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/__init__.py
+-rw-r--r--   0        0        0     4710 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/dynamic_pusher.py
+-rw-r--r--   0        0        0     2296 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/live_pusher.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/add_sub.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0        0        0     1551 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/sub_list.py
+-rw-r--r--   0        0        0     8200 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/__init__.py
+-rw-r--r--   0        0        0     6922 2023-06-27 09:18:54.507058 haruka-bot-1.6.0.post1/haruka_bot/utils/browser.py
+-rw-r--r--   0        0        0     4887 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/captcha.py
+-rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     7316 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post1/haruka_bot/utils/mobile.js
+-rw-r--r--   0        0        0       97 2023-06-27 09:19:31.036443 haruka-bot-1.6.0.post1/haruka_bot/version.py
+-rw-r--r--   0        0        0     1545 2023-06-27 09:03:26.103394 haruka-bot-1.6.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post1/PKG-INFO
```

### Comparing `haruka-bot-1.6.0/LICENSE` & `haruka-bot-1.6.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/README.md` & `haruka-bot-1.6.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/cli/bot.py` & `haruka-bot-1.6.0.post1/haruka_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/cli/utils.py` & `haruka-bot-1.6.0.post1/haruka_bot/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     file_path = Path("./.env.prod").resolve()
     if file_path.exists():
         return
 
     if any(Path.cwd().iterdir()):
         print("文件夹不为空，请更换空文件夹后重试")
         import sys
+
         sys.exit()
 
     while True:
         try:
             superusers = click.prompt(
                 "主人QQ号 (多个使用空格分开)", default="", show_default=False
             )
```

### Comparing `haruka-bot-1.6.0/haruka_bot/config.py` & `haruka-bot-1.6.0.post1/haruka_bot/config.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/database/db.py` & `haruka-bot-1.6.0.post1/haruka_bot/database/db.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/database/models.py` & `haruka-bot-1.6.0.post1/haruka_bot/database/models.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/libs/dynamic/__init__.py` & `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Optional
 from nonebot.adapters.onebot.v11.message import MessageSegment, Message
 from pydantic import BaseModel, root_validator
+
 # from pydantic import Json
 
 from .desc import Desc
+
 # from .card import Card
 # from .display import Display
 
 
 class Dynamic(BaseModel):
     desc: Desc
     # card: Json[Card]  # type: ignore
```

### Comparing `haruka-bot-1.6.0/haruka_bot/libs/dynamic/card.py` & `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/card.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
     author: Optional[Info]
 
     cover: Optional[str]
     area_v2_name: Optional[str]
 
     apiSeasonInfo: Optional[APISeasonInfo]
 
-    new_desc: Optional[str]
+    new_desc: Optional[str]
```

### Comparing `haruka-bot-1.6.0/haruka_bot/libs/dynamic/desc.py` & `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/desc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     # stype: int
     # r_type: int
     # inner_id: int
     # status: int
     # dynamic_id_str: str
     # pre_dy_id_str: str
     # orig_dy_id_str: str
-    # rid_str: str
+    # rid_str: str
```

### Comparing `haruka-bot-1.6.0/haruka_bot/libs/dynamic/display.py` & `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     id: int
     text: str
     url: str
 
 
 class EmojiInfo(BaseModel):
     """emoji 信息"""
+
     emoji_details: List[EmojiDetail]
 
 
 class DescFirst(BaseModel):
     text: str
```

### Comparing `haruka-bot-1.6.0/haruka_bot/libs/dynamic/user_profile.py` & `haruka-bot-1.6.0.post1/haruka_bot/libs/dynamic/user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 class Info(BaseModel):
     """用户信息"""
+
     uid: Optional[int]
     uname: Optional[str]
     face: Optional[str]
     head_url: Optional[str]
     name: Optional[str]
 
 
 class LevelInfo(BaseModel):
     """等级信息"""
+
     current_level: Optional[int]
 
 
 class Pendant(BaseModel):
     """挂件"""
+
     pid: int
     name: str
     image: str
 
 
 class OfficialVerify(BaseModel):
     """账号认证信息"""
+
     type: int
     desc: str
 
 
 class Card(BaseModel):
     official_verify: OfficialVerify
 
 
 class VIP(BaseModel):
     """大会员信息"""
+
     vipType: int
     nickname_color: str
 
 
 class UserProfile(BaseModel):
     info: Info
     level_info: Optional[LevelInfo]
     pendant: Optional[Pendant]
     card: Optional[Card]
-    vip: Optional[VIP]
+    vip: Optional[VIP]
```

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/at/at_off.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/at/at_on.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/at/at_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/auto_agree.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_agree.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/auto_delete.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/auto_delete.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_off.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_on.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/dynamic/dynamic_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/help.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/help.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/live/live_off.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/live/live_on.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/live/live_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_off.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_on.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/permission/permission_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/pusher/dynamic_pusher.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/dynamic_pusher.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/pusher/live_pusher.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/pusher/live_pusher.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/sub/add_sub.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/add_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/sub/delete_sub.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/delete_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/plugins/sub/sub_list.py` & `haruka-bot-1.6.0.post1/haruka_bot/plugins/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/utils/__init__.py` & `haruka-bot-1.6.0.post1/haruka_bot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/utils/browser.py` & `haruka-bot-1.6.0.post1/haruka_bot/utils/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
         ),
         viewport={"width": 460, "height": 780},
     )
     try:
         await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
         if plugin_config.haruka_captcha_address:
-            page = await resolve_captcha(url,page)
+            page = await resolve_captcha(url, page)
         else:
             await page.goto(
                 url,
                 wait_until="networkidle",
                 timeout=plugin_config.haruka_dynamic_timeout * 1000,
             )
         # 动态被删除或者进审核了
```

### Comparing `haruka-bot-1.6.0/haruka_bot/utils/captcha.py` & `haruka-bot-1.6.0.post1/haruka_bot/utils/captcha.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/utils/fonts_provider.py` & `haruka-bot-1.6.0.post1/haruka_bot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/haruka_bot/utils/mobile.js` & `haruka-bot-1.6.0.post1/haruka_bot/utils/mobile.js`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0/pyproject.toml` & `haruka-bot-1.6.0.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 authors = [
     { name = "SK-415", email = "2967923486@qq.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "click>=8.1.3",
-    "httpx>=0.24.0",
+    "httpx>=0.24.1",
     "nonebot-adapter-onebot>=2.2.3",
-    "nonebot-plugin-apscheduler>=0.2.0",
-    "nonebot2[fastapi]>=2.0.0rc4",
-    "playwright>=1.33.0",
-    "pydantic>=1.10.7",
+    "nonebot-plugin-apscheduler>=0.3.0",
+    "nonebot2[fastapi]>=2.0.0",
+    "playwright>=1.35.0",
+    "pydantic>=1.10.9",
     "python-dotenv>=1.0.0",
     "tortoise-orm[asyncpg]>=0.19.3",
-    "bilireq>=0.2.5",
+    "bilireq>=0.2.6",
     "packaging>=23.1",
     "nonebot-plugin-guild-patch>=0.2.3",
     "msvc-runtime>=14.34.31931; sys_platform == \"win32\"",
 ]
 dynamic = []
 name = "haruka-bot"
 description = "Push dynamics and live informations from bilibili to QQ. Based on nonebot2."
@@ -25,15 +25,15 @@
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bilibili",
     "bot",
 ]
-version = "1.6.0"
+version = "1.6.0.post1"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/SK-415/HarukaBot"
 repository = "https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot"
@@ -47,16 +47,14 @@
     "nonebot-plugin-gocqhttp>=0.6.10",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "haruka_bot/version.py"
 
-[tool.pdm.build]
-
 [tool.nonebot]
 adapters = [
     { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
 ]
 plugins = [
     "haruka_bot",
     "nonebot_plugin_gocqhttp",
```

### Comparing `haruka-bot-1.6.0/PKG-INFO` & `haruka-bot-1.6.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka-bot
-Version: 1.6.0
+Version: 1.6.0.post1
 Summary: Push dynamics and live informations from bilibili to QQ. Based on nonebot2.
 License: AGPL-3.0-or-later
 Keywords: nonebot,nonebot2,qqbot,bilibili,bot
 Author-email: SK-415 <2967923486@qq.com>
 Requires-Python: >=3.8,<4.0
 Project-URL: documentation, https://github.com/SK-415/HarukaBot#readme
 Project-URL: homepage, https://github.com/SK-415/HarukaBot
```

