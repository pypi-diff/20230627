# Comparing `tmp/haruka-bot-1.5.4.tar.gz` & `tmp/haruka-bot-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka-bot-1.5.4.tar", last modified: Thu May  4 22:55:35 2023, max compression
+gzip compressed data, was "haruka-bot-1.6.0.tar", last modified: Tue Jun 27 08:51:15 2023, max compression
```

## Comparing `haruka-bot-1.5.4.tar` & `haruka-bot-1.6.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0      263 2023-05-01 05:18:50.706789 haruka-bot-1.5.4/haruka_bot/__init__.py
--rw-r--r--   0        0        0       61 2022-11-22 23:51:45.819393 haruka-bot-1.5.4/haruka_bot/__main__.py
--rw-r--r--   0        0        0      189 2022-11-22 23:51:45.823393 haruka-bot-1.5.4/haruka_bot/cli/__init__.py
--rw-r--r--   0        0        0      734 2022-11-22 23:51:45.827394 haruka-bot-1.5.4/haruka_bot/cli/bot.py
--rw-r--r--   0        0        0     1169 2022-11-22 23:51:45.829393 haruka-bot-1.5.4/haruka_bot/cli/utils.py
--rw-r--r--   0        0        0     1363 2023-05-04 21:46:30.610407 haruka-bot-1.5.4/haruka_bot/config.py
--rw-r--r--   0        0        0       49 2022-11-26 12:34:38.721371 haruka-bot-1.5.4/haruka_bot/database/__init__.py
--rw-r--r--   0        0        0    10476 2023-05-04 21:32:01.721909 haruka-bot-1.5.4/haruka_bot/database/db.py
--rw-r--r--   0        0        0     2017 2023-02-13 19:22:21.855406 haruka-bot-1.5.4/haruka_bot/database/models.py
--rw-r--r--   0        0        0       30 2022-11-22 23:51:45.847394 haruka-bot-1.5.4/haruka_bot/libs/__init__.py
--rw-r--r--   0        0        0     1464 2022-11-22 23:51:45.854393 haruka-bot-1.5.4/haruka_bot/libs/dynamic/__init__.py
--rw-r--r--   0        0        0     1084 2022-11-22 23:51:45.859394 haruka-bot-1.5.4/haruka_bot/libs/dynamic/card.py
--rw-r--r--   0        0        0      597 2022-11-22 23:51:45.863395 haruka-bot-1.5.4/haruka_bot/libs/dynamic/desc.py
--rw-r--r--   0        0        0     1023 2022-11-22 23:51:45.866393 haruka-bot-1.5.4/haruka_bot/libs/dynamic/display.py
--rw-r--r--   0        0        0      810 2022-11-22 23:51:45.870393 haruka-bot-1.5.4/haruka_bot/libs/dynamic/user_profile.py
--rw-r--r--   0        0        0      465 2023-05-01 05:18:50.709789 haruka-bot-1.5.4/haruka_bot/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 05:18:50.709789 haruka-bot-1.5.4/haruka_bot/plugins/at/__init__.py
--rw-r--r--   0        0        0     1478 2023-05-01 05:18:50.710789 haruka-bot-1.5.4/haruka_bot/plugins/at/at_off.py
--rw-r--r--   0        0        0     1469 2023-05-01 05:18:50.711789 haruka-bot-1.5.4/haruka_bot/plugins/at/at_on.py
--rw-r--r--   0        0        0      678 2022-11-22 23:51:45.892393 haruka-bot-1.5.4/haruka_bot/plugins/auto_agree.py
--rw-r--r--   0        0        0      897 2023-02-13 19:22:21.859410 haruka-bot-1.5.4/haruka_bot/plugins/auto_delete.py
--rw-r--r--   0        0        0        0 2023-05-01 05:18:50.711789 haruka-bot-1.5.4/haruka_bot/plugins/dynamic/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-01 05:18:50.712789 haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_off.py
--rw-r--r--   0        0        0     1076 2023-05-01 05:18:50.712789 haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_on.py
--rw-r--r--   0        0        0      755 2023-05-01 05:18:50.713791 haruka-bot-1.5.4/haruka_bot/plugins/help.py
--rw-r--r--   0        0        0        0 2023-05-01 05:18:50.713791 haruka-bot-1.5.4/haruka_bot/plugins/live/__init__.py
--rw-r--r--   0        0        0     1058 2023-05-01 05:18:50.714789 haruka-bot-1.5.4/haruka_bot/plugins/live/live_off.py
--rw-r--r--   0        0        0     1049 2023-05-01 05:18:50.715792 haruka-bot-1.5.4/haruka_bot/plugins/live/live_on.py
--rw-r--r--   0        0        0        0 2023-05-01 05:18:50.715792 haruka-bot-1.5.4/haruka_bot/plugins/permission/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-01 05:18:50.716789 haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_off.py
--rw-r--r--   0        0        0     1232 2023-05-01 05:18:50.717790 haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_on.py
--rw-r--r--   0        0        0       59 2023-05-01 05:18:50.717790 haruka-bot-1.5.4/haruka_bot/plugins/pusher/__init__.py
--rw-r--r--   0        0        0     4847 2023-05-04 22:04:19.503423 haruka-bot-1.5.4/haruka_bot/plugins/pusher/dynamic_pusher.py
--rw-r--r--   0        0        0     2360 2023-05-01 05:18:50.719789 haruka-bot-1.5.4/haruka_bot/plugins/pusher/live_pusher.py
--rw-r--r--   0        0        0        0 2023-05-01 05:18:50.719789 haruka-bot-1.5.4/haruka_bot/plugins/sub/__init__.py
--rw-r--r--   0        0        0     2113 2023-05-01 05:18:50.720789 haruka-bot-1.5.4/haruka_bot/plugins/sub/add_sub.py
--rw-r--r--   0        0        0     1058 2023-05-01 05:18:50.721790 haruka-bot-1.5.4/haruka_bot/plugins/sub/delete_sub.py
--rw-r--r--   0        0        0     1594 2023-05-01 05:18:50.721790 haruka-bot-1.5.4/haruka_bot/plugins/sub/sub_list.py
--rw-r--r--   0        0        0     8441 2023-05-01 05:18:50.722790 haruka-bot-1.5.4/haruka_bot/utils/__init__.py
--rw-r--r--   0        0        0     6952 2023-05-01 05:18:50.723790 haruka-bot-1.5.4/haruka_bot/utils/browser.py
--rw-r--r--   0        0        0      730 2023-05-01 05:18:50.723790 haruka-bot-1.5.4/haruka_bot/utils/fonts_provider.py
--rw-r--r--   0        0        0     7512 2023-05-01 05:18:50.724790 haruka-bot-1.5.4/haruka_bot/utils/mobile.js
--rw-r--r--   0        0        0       96 2023-05-04 22:55:27.792965 haruka-bot-1.5.4/haruka_bot/version.py
--rw-r--r--   0        0        0    34522 2022-11-22 23:51:45.311395 haruka-bot-1.5.4/LICENSE
--rw-r--r--   0        0        0     1560 2023-05-04 22:20:40.010725 haruka-bot-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     2837 2023-05-01 05:18:50.695791 haruka-bot-1.5.4/README.md
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 haruka-bot-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-06-27 08:46:55.526760 haruka-bot-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2790 2023-06-27 08:46:55.526760 haruka-bot-1.6.0/README.md
+-rw-r--r--   0        0        0      253 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/__main__.py
+-rw-r--r--   0        0        0      189 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/cli/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/cli/bot.py
+-rw-r--r--   0        0        0     1169 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/cli/utils.py
+-rw-r--r--   0        0        0     1390 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/config.py
+-rw-r--r--   0        0        0       49 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/database/__init__.py
+-rw-r--r--   0        0        0    10155 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/database/db.py
+-rw-r--r--   0        0        0     1936 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/database/models.py
+-rw-r--r--   0        0        0       30 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/__init__.py
+-rw-r--r--   0        0        0     1464 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/card.py
+-rw-r--r--   0        0        0      597 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/desc.py
+-rw-r--r--   0        0        0     1023 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/display.py
+-rw-r--r--   0        0        0      810 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/libs/dynamic/user_profile.py
+-rw-r--r--   0        0        0      456 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:47:26.570760 haruka-bot-1.6.0/haruka_bot/plugins/at/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/at/at_off.py
+-rw-r--r--   0        0        0     1421 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/at/at_on.py
+-rw-r--r--   0        0        0      678 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/auto_agree.py
+-rw-r--r--   0        0        0      875 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/auto_delete.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/dynamic/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_off.py
+-rw-r--r--   0        0        0     1039 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_on.py
+-rw-r--r--   0        0        0      734 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/help.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/live/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/live/live_off.py
+-rw-r--r--   0        0        0     1012 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/permission/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_off.py
+-rw-r--r--   0        0        0     1201 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_on.py
+-rw-r--r--   0        0        0       58 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/pusher/__init__.py
+-rw-r--r--   0        0        0     4710 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/pusher/dynamic_pusher.py
+-rw-r--r--   0        0        0     2296 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/pusher/live_pusher.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:47:26.574760 haruka-bot-1.6.0/haruka_bot/plugins/sub/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/sub/add_sub.py
+-rw-r--r--   0        0        0     1021 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0        0        0     1551 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/plugins/sub/sub_list.py
+-rw-r--r--   0        0        0     8200 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/__init__.py
+-rw-r--r--   0        0        0     6921 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/browser.py
+-rw-r--r--   0        0        0     4887 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/captcha.py
+-rw-r--r--   0        0        0      702 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     7316 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/utils/mobile.js
+-rw-r--r--   0        0        0       92 2023-06-27 08:46:55.562760 haruka-bot-1.6.0/haruka_bot/version.py
+-rw-r--r--   0        0        0     1560 2023-06-27 08:46:55.566760 haruka-bot-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 haruka-bot-1.6.0/PKG-INFO
```

### Comparing `haruka-bot-1.5.4/haruka_bot/cli/bot.py` & `haruka-bot-1.6.0/haruka_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/cli/utils.py` & `haruka-bot-1.6.0/haruka_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/config.py` & `haruka-bot-1.6.0/haruka_bot/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from typing import List, Optional
-
-from nonebot import get_driver
-from pydantic import BaseSettings, validator
-from pydantic.fields import ModelField
-
-
-# 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
-class Config(BaseSettings):
-    fastapi_reload: bool = False
-    haruka_dir: Optional[str] = None
-    haruka_to_me: bool = True
-    haruka_live_off_notify: bool = False
-    haruka_proxy: Optional[str] = None
-    haruka_interval: int = 10
-    haruka_live_interval: int = haruka_interval
-    haruka_dynamic_interval: int = 0
-    haruka_dynamic_at: bool = False
-    haruka_screenshot_style: str = "mobile"
-    haruka_dynamic_timeout: int = 30
-    haruka_dynamic_font_source: str = "system"
-    haruka_dynamic_font: Optional[str] = "Noto Sans CJK SC"
-    haruka_command_prefix: str = ""
-    # 频道管理员身份组
-    haruka_guild_admin_roles: List[str] = ["频道主", "超级管理员"]
-
-    @validator("haruka_interval", "haruka_live_interval", "haruka_dynamic_interval")
-    def non_negative(cls, v: int, field: ModelField):
-        """定时器为负返回默认值"""
-        if v < 1:
-            return field.default
-        return v
-
-    class Config:
-        extra = "ignore"
-
-
-global_config = get_driver().config
-plugin_config = Config.parse_obj(global_config)
+from typing import List, Optional
+
+from nonebot import get_driver
+from pydantic import BaseSettings, validator
+from pydantic.fields import ModelField
+
+
+# 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
+class Config(BaseSettings):
+    fastapi_reload: bool = False
+    haruka_dir: Optional[str] = None
+    haruka_to_me: bool = True
+    haruka_live_off_notify: bool = False
+    haruka_proxy: Optional[str] = None
+    haruka_interval: int = 10
+    haruka_live_interval: int = haruka_interval
+    haruka_dynamic_interval: int = 0
+    haruka_dynamic_at: bool = False
+    haruka_screenshot_style: str = "mobile"
+    haruka_captcha_address: str = "https://captcha-cd.ngworks.cn"
+    haruka_dynamic_timeout: int = 30
+    haruka_dynamic_font_source: str = "system"
+    haruka_dynamic_font: Optional[str] = "Noto Sans CJK SC"
+    haruka_command_prefix: str = ""
+    # 频道管理员身份组
+    haruka_guild_admin_roles: List[str] = ["频道主", "超级管理员"]
+
+    @validator("haruka_interval", "haruka_live_interval", "haruka_dynamic_interval")
+    def non_negative(cls, v: int, field: ModelField):
+        """定时器为负返回默认值"""
+        if v < 1:
+            return field.default
+        return v
+
+    class Config:
+        extra = "ignore"
+
+
+global_config = get_driver().config
+plugin_config = Config.parse_obj(global_config)
```

### Comparing `haruka-bot-1.5.4/haruka_bot/libs/dynamic/__init__.py` & `haruka-bot-1.6.0/haruka_bot/libs/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/libs/dynamic/card.py` & `haruka-bot-1.6.0/haruka_bot/libs/dynamic/card.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/libs/dynamic/desc.py` & `haruka-bot-1.6.0/haruka_bot/libs/dynamic/desc.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/libs/dynamic/display.py` & `haruka-bot-1.6.0/haruka_bot/libs/dynamic/display.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/libs/dynamic/user_profile.py` & `haruka-bot-1.6.0/haruka_bot/libs/dynamic/user_profile.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/at/at_on.py` & `haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_on.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,31 @@
-from typing import Union
-
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
-from nonebot.params import ArgPlainText
-from nonebot.permission import SUPERUSER
-from nonebot_plugin_guild_patch import GuildMessageEvent
-
-from ...config import plugin_config
-from ...database import DB as db
-from ...utils import (
-    GUILD_ADMIN,
-    get_type_id,
-    group_only,
-    handle_uid,
-    on_command,
-    to_me,
-    uid_check,
-)
-
-at_on = on_command(
-    "开启全体",
-    rule=to_me(),
-    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
-    priority=5,
-)
-at_on.__doc__ = """开启全体 UID"""
-
-at_on.handle()(group_only)
-at_on.handle()(handle_uid)
-at_on.got("uid", prompt="请输入要开启全体的UID")(uid_check)
-
-
-@at_on.handle()
-async def _(
-    event: Union[GroupMessageEvent, GuildMessageEvent], uid: str = ArgPlainText("uid")
-):
-    """根据 UID 开启全体"""
-    if await db.set_sub(
-        "at", True, uid=uid, type=event.message_type, type_id=await get_type_id(event)
-    ):
-        user = await db.get_user(uid=uid)
-        assert user is not None
-        await at_on.finish(
-            f"已开启 {user.name}（{user.uid}）"
-            f"{'直播推送' if not plugin_config.haruka_dynamic_at else ''}的@全体"
-        )
-    await at_on.finish(f"UID（{uid}）未关注，请先关注后再操作")
+from typing import Union
+
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
+from nonebot.permission import SUPERUSER
+from nonebot_plugin_guild_patch import GuildMessageEvent
+
+from ...database import DB as db
+from ...utils import GUILD_ADMIN, group_only, on_command, to_me
+
+permission_on = on_command(
+    "开启权限",
+    rule=to_me(),
+    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
+    priority=5,
+)
+permission_on.__doc__ = """开启权限"""
+
+permission_on.handle()(group_only)
+
+
+@permission_on.handle()
+async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
+    """开启当前群权限"""
+    if isinstance(event, GuildMessageEvent):
+        if await db.set_guild_permission(event.guild_id, event.channel_id, True):
+            await permission_on.finish("已开启权限，只有管理员和主人可以操作")
+    else:
+        if await db.set_permission(event.group_id, True):
+            await permission_on.finish("已开启权限，只有管理员和主人可以操作")
+    await permission_on.finish("权限已经开启了，只有管理员和主人可以操作")
```

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/auto_agree.py` & `haruka-bot-1.6.0/haruka_bot/plugins/auto_agree.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/auto_delete.py` & `haruka-bot-1.6.0/haruka_bot/plugins/auto_delete.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Union
-
-from nonebot import on_notice
-from nonebot.adapters.onebot.v11 import GroupDecreaseNoticeEvent
-from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent
-
-from ..database import DB as db
-from ..utils import get_type_id
-
-group_decrease = on_notice(priority=5)
-
-
-@group_decrease.handle()
-async def _(event: Union[GroupDecreaseNoticeEvent, ChannelDestroyedNoticeEvent]):
-    """退群时，自动删除该群订阅列表"""
-    if isinstance(event, GroupDecreaseNoticeEvent):
-        if event.self_id == event.user_id:
-            await db.delete_sub_list(type="group", type_id=event.group_id)
-            await db.delete_group(id=event.group_id)
-    elif isinstance(event, ChannelDestroyedNoticeEvent):
-        await db.delete_sub_list(type="guild", type_id=await get_type_id(event))
-        await db.delete_guild(id=await get_type_id(event))
+from typing import Union
+
+from nonebot import on_notice
+from nonebot.adapters.onebot.v11 import GroupDecreaseNoticeEvent
+from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent
+
+from ..database import DB as db
+from ..utils import get_type_id
+
+group_decrease = on_notice(priority=5)
+
+
+@group_decrease.handle()
+async def _(event: Union[GroupDecreaseNoticeEvent, ChannelDestroyedNoticeEvent]):
+    """退群时，自动删除该群订阅列表"""
+    if isinstance(event, GroupDecreaseNoticeEvent):
+        if event.self_id == event.user_id:
+            await db.delete_sub_list(type="group", type_id=event.group_id)
+            await db.delete_group(id=event.group_id)
+    elif isinstance(event, ChannelDestroyedNoticeEvent):
+        await db.delete_sub_list(type="guild", type_id=await get_type_id(event))
+        await db.delete_guild(id=await get_type_id(event))
```

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_on.py` & `haruka-bot-1.6.0/haruka_bot/plugins/dynamic/dynamic_on.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from nonebot.adapters.onebot.v11.event import MessageEvent
-from nonebot.params import ArgPlainText
-
-from ...database import DB as db
-from ...utils import (
-    get_type_id,
-    handle_uid,
-    on_command,
-    permission_check,
-    to_me,
-    uid_check,
-)
-
-dynamic_on = on_command("开启动态", rule=to_me(), priority=5)
-dynamic_on.__doc__ = """开启动态 UID"""
-
-dynamic_on.handle()(permission_check)
-
-dynamic_on.handle()(handle_uid)
-
-dynamic_on.got("uid", prompt="请输入要开启动态的UID")(uid_check)
-
-
-@dynamic_on.handle()
-async def _(event: MessageEvent, uid: str = ArgPlainText("uid")):
-    """根据 UID 开启动态"""
-    if await db.set_sub(
-        "dynamic",
-        True,
-        uid=uid,
-        type=event.message_type,
-        type_id=await get_type_id(event),
-    ):
-        user = await db.get_user(uid=uid)
-        assert user is not None
-        await dynamic_on.finish(f"已开启 {user.name}（{user.uid}）的动态推送")
-    await dynamic_on.finish(f"UID（{uid}）未关注，请先关注后再操作")
+from nonebot.adapters.onebot.v11.event import MessageEvent
+from nonebot.params import ArgPlainText
+
+from ...database import DB as db
+from ...utils import (
+    get_type_id,
+    handle_uid,
+    on_command,
+    permission_check,
+    to_me,
+    uid_check,
+)
+
+dynamic_on = on_command("开启动态", rule=to_me(), priority=5)
+dynamic_on.__doc__ = """开启动态 UID"""
+
+dynamic_on.handle()(permission_check)
+
+dynamic_on.handle()(handle_uid)
+
+dynamic_on.got("uid", prompt="请输入要开启动态的UID")(uid_check)
+
+
+@dynamic_on.handle()
+async def _(event: MessageEvent, uid: str = ArgPlainText("uid")):
+    """根据 UID 开启动态"""
+    if await db.set_sub(
+        "dynamic",
+        True,
+        uid=uid,
+        type=event.message_type,
+        type_id=await get_type_id(event),
+    ):
+        user = await db.get_user(uid=uid)
+        assert user is not None
+        await dynamic_on.finish(f"已开启 {user.name}（{user.uid}）的动态推送")
+    await dynamic_on.finish(f"UID（{uid}）未关注，请先关注后再操作")
```

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/live/live_off.py` & `haruka-bot-1.6.0/haruka_bot/plugins/live/live_off.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from nonebot.adapters.onebot.v11.event import MessageEvent
-from nonebot.params import ArgPlainText
-
-from ...database import DB as db
-from ...utils import (
-    get_type_id,
-    handle_uid,
-    on_command,
-    permission_check,
-    to_me,
-    uid_check,
-)
-
-live_off = on_command("关闭直播", rule=to_me(), priority=5)
-live_off.__doc__ = """关闭直播 UID"""
-
-live_off.handle()(permission_check)
-
-live_off.handle()(handle_uid)
-
-live_off.got("uid", prompt="请输入要关闭直播的UID")(uid_check)
-
-
-@live_off.handle()
-async def _(event: MessageEvent, uid: str = ArgPlainText("uid")):
-    """根据 UID 关闭直播"""
-    if await db.set_sub(
-        "live",
-        False,
-        uid=uid,
-        type=event.message_type,
-        type_id=await get_type_id(event),
-    ):
-        user = await db.get_user(uid=uid)
-        assert user is not None
-        await live_off.finish(f"已关闭 {user.name}（{user.uid}）的直播推送")
-    await live_off.finish(f"UID（{uid}）未关注，请先关注后再操作")
+from nonebot.adapters.onebot.v11.event import MessageEvent
+from nonebot.params import ArgPlainText
+
+from ...database import DB as db
+from ...utils import (
+    get_type_id,
+    handle_uid,
+    on_command,
+    permission_check,
+    to_me,
+    uid_check,
+)
+
+live_off = on_command("关闭直播", rule=to_me(), priority=5)
+live_off.__doc__ = """关闭直播 UID"""
+
+live_off.handle()(permission_check)
+
+live_off.handle()(handle_uid)
+
+live_off.got("uid", prompt="请输入要关闭直播的UID")(uid_check)
+
+
+@live_off.handle()
+async def _(event: MessageEvent, uid: str = ArgPlainText("uid")):
+    """根据 UID 关闭直播"""
+    if await db.set_sub(
+        "live",
+        False,
+        uid=uid,
+        type=event.message_type,
+        type_id=await get_type_id(event),
+    ):
+        user = await db.get_user(uid=uid)
+        assert user is not None
+        await live_off.finish(f"已关闭 {user.name}（{user.uid}）的直播推送")
+    await live_off.finish(f"UID（{uid}）未关注，请先关注后再操作")
```

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_off.py` & `haruka-bot-1.6.0/haruka_bot/plugins/permission/permission_off.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Union
-
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
-from nonebot.permission import SUPERUSER
-from nonebot_plugin_guild_patch import GuildMessageEvent
-
-from ...database import DB as db
-from ...utils import GUILD_ADMIN, group_only, on_command, to_me
-
-permission_off = on_command(
-    "关闭权限",
-    rule=to_me(),
-    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
-    priority=5,
-)
-permission_off.__doc__ = """关闭权限"""
-
-permission_off.handle()(group_only)
-
-
-@permission_off.handle()
-async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
-    """关闭当前群权限"""
-    if isinstance(event, GuildMessageEvent):
-        if await db.set_guild_permission(event.guild_id, event.channel_id, False):
-            await permission_off.finish("已开启权限，只有管理员和主人可以操作")
-    else:
-        if await db.set_permission(event.group_id, False):
-            await permission_off.finish("已关闭权限，所有人均可操作")
-    await permission_off.finish("权限已经关闭了，所有人均可操作")
+from typing import Union
+
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
+from nonebot.permission import SUPERUSER
+from nonebot_plugin_guild_patch import GuildMessageEvent
+
+from ...database import DB as db
+from ...utils import GUILD_ADMIN, group_only, on_command, to_me
+
+permission_off = on_command(
+    "关闭权限",
+    rule=to_me(),
+    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
+    priority=5,
+)
+permission_off.__doc__ = """关闭权限"""
+
+permission_off.handle()(group_only)
+
+
+@permission_off.handle()
+async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
+    """关闭当前群权限"""
+    if isinstance(event, GuildMessageEvent):
+        if await db.set_guild_permission(event.guild_id, event.channel_id, False):
+            await permission_off.finish("已开启权限，只有管理员和主人可以操作")
+    else:
+        if await db.set_permission(event.group_id, False):
+            await permission_off.finish("已关闭权限，所有人均可操作")
+    await permission_off.finish("权限已经关闭了，所有人均可操作")
```

### Comparing `haruka-bot-1.5.4/haruka_bot/plugins/sub/sub_list.py` & `haruka-bot-1.6.0/haruka_bot/plugins/sub/sub_list.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from nonebot.adapters.onebot.v11 import Bot
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent, MessageEvent
-
-from ...database import DB as db
-from ...utils import get_type_id, on_command, permission_check, to_me
-
-sub_list = on_command("关注列表", aliases={"主播列表"}, rule=to_me(), priority=5)
-sub_list.__doc__ = """关注列表"""
-
-sub_list.handle()(permission_check)
-
-
-@sub_list.handle()
-async def _(event: MessageEvent, bot: Bot):
-    """发送当前位置的订阅列表"""
-    message = "关注列表（所有群/好友都是分开的）\n\n"
-    subs = await db.get_sub_list(event.message_type, await get_type_id(event))
-    for sub in subs:
-        user = await db.get_user(uid=sub.uid)
-        assert user is not None
-        message += (
-            f"{user.name}（{user.uid}）"
-            f"直播：{'开' if sub.live else '关'}，"
-            f"动态：{'开' if sub.dynamic else '关'}，"
-            # TODO 私聊不显示全体
-            f"全体：{'开' if sub.at else '关'}\n"
-        )
-    if len(message.splitlines()) > 8 and isinstance(event, GroupMessageEvent):
-        await bot.send_group_forward_msg(
-            group_id=event.group_id,
-            messages=[
-                {
-                    "type": "node",
-                    "data": {
-                        "name": "HarukaBot",
-                        "uin": bot.self_id,
-                        "content": message,
-                    },
-                }
-            ],
-        )
-    else:
-        await sub_list.finish(message)
+from nonebot.adapters.onebot.v11 import Bot
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent, MessageEvent
+
+from ...database import DB as db
+from ...utils import get_type_id, on_command, permission_check, to_me
+
+sub_list = on_command("关注列表", aliases={"主播列表"}, rule=to_me(), priority=5)
+sub_list.__doc__ = """关注列表"""
+
+sub_list.handle()(permission_check)
+
+
+@sub_list.handle()
+async def _(event: MessageEvent, bot: Bot):
+    """发送当前位置的订阅列表"""
+    message = "关注列表（所有群/好友都是分开的）\n\n"
+    subs = await db.get_sub_list(event.message_type, await get_type_id(event))
+    for sub in subs:
+        user = await db.get_user(uid=sub.uid)
+        assert user is not None
+        message += (
+            f"{user.name}（{user.uid}）"
+            f"直播：{'开' if sub.live else '关'}，"
+            f"动态：{'开' if sub.dynamic else '关'}，"
+            # TODO 私聊不显示全体
+            f"全体：{'开' if sub.at else '关'}\n"
+        )
+    if len(message.splitlines()) > 8 and isinstance(event, GroupMessageEvent):
+        await bot.send_group_forward_msg(
+            group_id=event.group_id,
+            messages=[
+                {
+                    "type": "node",
+                    "data": {
+                        "name": "HarukaBot",
+                        "uin": bot.self_id,
+                        "content": message,
+                    },
+                }
+            ],
+        )
+    else:
+        await sub_list.finish(message)
```

### Comparing `haruka-bot-1.5.4/haruka_bot/utils/__init__.py` & `haruka-bot-1.6.0/haruka_bot/utils/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-import asyncio
-import sys
-from pathlib import Path
-from typing import Union
-
-import httpx
-import nonebot
-from nonebot import on_command as _on_command
-from nonebot import require
-from nonebot.adapters.onebot.v11 import (
-    ActionFailed,
-    Bot,
-    Message,
-    MessageEvent,
-    MessageSegment,
-    NetworkError,
-)
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent, PrivateMessageEvent
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
-from nonebot.exception import FinishedException
-from nonebot.log import logger
-from nonebot.matcher import Matcher
-from nonebot.params import ArgPlainText, CommandArg, RawCommand
-from nonebot.permission import SUPERUSER, Permission
-from nonebot.rule import Rule
-from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent, GuildMessageEvent
-
-from ..config import plugin_config
-
-
-def get_path(*other):
-    """获取数据文件绝对路径"""
-    if plugin_config.haruka_dir:
-        dir_path = Path(plugin_config.haruka_dir).resolve()
-    else:
-        dir_path = Path.cwd().joinpath("data")
-        # dir_path = Path.cwd().joinpath('data', 'haruka_bot')
-    return str(dir_path.joinpath(*other))
-
-
-async def handle_uid(
-    matcher: Matcher,
-    command_arg: Message = CommandArg(),
-):
-    uid = command_arg.extract_plain_text().strip()
-    if uid:
-        matcher.set_arg("uid", command_arg)
-
-
-async def uid_check(
-    matcher: Matcher,
-    uid: str = ArgPlainText("uid"),
-):
-    uid = uid.strip()
-    if not uid.isdecimal():
-        await matcher.finish("UID 必须为纯数字")
-    matcher.set_arg("uid", Message(uid))
-
-
-async def _guild_admin(bot: Bot, event: GuildMessageEvent):
-    roles = set(
-        role["role_name"]
-        for role in (
-            await bot.get_guild_member_profile(
-                guild_id=event.guild_id, user_id=event.user_id
-            )
-        )["roles"]
-    )
-    return bool(roles & set(plugin_config.haruka_guild_admin_roles))
-
-
-GUILD_ADMIN: Permission = Permission(_guild_admin)
-
-
-async def permission_check(
-    bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent, GuildMessageEvent]
-):
-    from ..database import DB as db
-
-    if isinstance(event, PrivateMessageEvent):
-        if event.sub_type == "group":  # 不处理群临时会话
-            raise FinishedException
-        return
-    if isinstance(event, GroupMessageEvent):
-        if not await db.get_group_admin(event.group_id):
-            return
-        if await (GROUP_ADMIN | GROUP_OWNER | SUPERUSER)(bot, event):
-            return
-    elif isinstance(event, GuildMessageEvent):
-        if not await db.get_guild_admin(event.guild_id, event.channel_id):
-            return
-        if await (GUILD_ADMIN | SUPERUSER)(bot, event):
-            return
-    await bot.send(event, "权限不足，目前只有管理员才能使用")
-    raise FinishedException
-
-
-async def group_only(
-    matcher: Matcher, event: PrivateMessageEvent, command: str = RawCommand()
-):
-    await matcher.finish(f"只有群里才能{command}")
-
-
-def to_me():
-    if plugin_config.haruka_to_me:
-        from nonebot.rule import to_me
-
-        return to_me()
-
-    async def _to_me() -> bool:
-        return True
-
-    return Rule(_to_me)
-
-
-async def safe_send(bot_id, send_type, type_id, message, at=False):
-    """发送出现错误时, 尝试重新发送, 并捕获异常且不会中断运行"""
-
-    async def _safe_send(bot, send_type, type_id, message):
-        if send_type == "guild":
-            from ..database import DB as db
-
-            guild = await db.get_guild(id=type_id)
-            assert guild
-            result = await bot.send_guild_channel_msg(
-                guild_id=guild.guild_id,
-                channel_id=guild.channel_id,
-                message=message,
-            )
-        else:
-            result = await bot.call_api(
-                "send_" + send_type + "_msg",
-                **{
-                    "message": message,
-                    "user_id" if send_type == "private" else "group_id": type_id,
-                },
-            )
-        return result
-
-    bots = nonebot.get_bots()
-    bot = bots.get(str(bot_id))
-    if bot is None:
-        logger.error(f"推送失败，Bot（{bot_id}）未连接，尝试使用其他 Bot 推送")
-        for bot_id, bot in bots.items():
-            if at and (
-                send_type == "guild"
-                or (await bot.get_group_at_all_remain(group_id=type_id))["can_at_all"]
-            ):
-                message = MessageSegment.at("all") + message
-            try:
-                result = await _safe_send(bot, send_type, type_id, message)
-                logger.info(f"尝试使用 Bot（{bot_id}）推送成功")
-                return result
-            except Exception:
-                continue
-        logger.error("尝试失败，所有 Bot 均无法推送")
-        return
-
-    if at and (
-        send_type == "guild"
-        or (await bot.get_group_at_all_remain(group_id=type_id))["can_at_all"]
-    ):
-        message = MessageSegment.at("all") + message
-
-    try:
-        return await _safe_send(bot, send_type, type_id, message)
-    except ActionFailed as e:
-        if e.info["msg"] == "GROUP_NOT_FOUND":
-            from ..database import DB as db
-
-            await db.delete_sub_list(type="group", type_id=type_id)
-            await db.delete_group(id=type_id)
-            logger.error(f"推送失败，群（{type_id}）不存在，已自动清理群订阅列表")
-        elif e.info["msg"] == "CHANNEL_NOT_FOUND":
-            from ..database import DB as db
-
-            guild = await db.get_guild(id=type_id)
-            assert guild
-            await db.delete_sub_list(type="guild", type_id=type_id)
-            await db.delete_guild(id=type_id)
-            logger.error(f"推送失败，频道（{guild.guild_id}|{guild.channel_id}）不存在，已自动清理频道订阅列表")
-        elif e.info["msg"] == "SEND_MSG_API_ERROR":
-            url = "https://haruka-bot.sk415.icu/usage/faq.html#机器人不发消息也没反应"
-            logger.error(f"推送失败，账号可能被风控（{url}），错误信息：{e.info}")
-        else:
-            logger.error(f"推送失败，未知错误，错误信息：{e.info}")
-    except NetworkError as e:
-        logger.error(f"推送失败，请检查网络连接，错误信息：{e.msg}")
-
-
-async def get_type_id(event: Union[MessageEvent, ChannelDestroyedNoticeEvent]):
-    if isinstance(event, GuildMessageEvent) or isinstance(
-        event, ChannelDestroyedNoticeEvent
-    ):
-        from ..database import DB as db
-
-        return await db.get_guild_type_id(event.guild_id, event.channel_id)
-    return event.group_id if isinstance(event, GroupMessageEvent) else event.user_id
-
-
-def check_proxy():
-    """检查代理是否有效"""
-    if plugin_config.haruka_proxy:
-        logger.info("检查代理是否有效")
-        try:
-            httpx.get(
-                "https://icanhazip.com/",
-                proxies={"all://": plugin_config.haruka_proxy},
-                timeout=2,
-            )
-        except Exception:
-            raise RuntimeError("加载失败，代理无法连接，请检查 HARUKA_PROXY 后重试")
-
-
-def on_startup():
-    """安装依赖并检查当前环境是否满足运行条件"""
-    if plugin_config.fastapi_reload and sys.platform == "win32":
-        raise ImportError("加载失败，Windows 必须设置 FASTAPI_RELOAD=false 才能正常运行 HarukaBot")
-    try:  # 如果开启 realod 只在第一次运行
-        asyncio.get_running_loop()
-    except RuntimeError:
-        from .browser import check_playwright_env, install
-
-        check_proxy()
-        install()
-        asyncio.get_event_loop().run_until_complete(check_playwright_env())
-        # 创建数据存储目录
-        if not Path(get_path()).is_dir():
-            Path(get_path()).mkdir(parents=True)
-
-
-def on_command(cmd, *args, **kwargs):
-    return _on_command(plugin_config.haruka_command_prefix + cmd, *args, **kwargs)
-
-
-PROXIES = {"all://": plugin_config.haruka_proxy}
-
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler  # noqa
-
-from .browser import get_dynamic_screenshot  # noqa
+import asyncio
+import sys
+from pathlib import Path
+from typing import Union
+
+import httpx
+import nonebot
+from nonebot import on_command as _on_command
+from nonebot import require
+from nonebot.adapters.onebot.v11 import (
+    ActionFailed,
+    Bot,
+    Message,
+    MessageEvent,
+    MessageSegment,
+    NetworkError,
+)
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent, PrivateMessageEvent
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
+from nonebot.exception import FinishedException
+from nonebot.log import logger
+from nonebot.matcher import Matcher
+from nonebot.params import ArgPlainText, CommandArg, RawCommand
+from nonebot.permission import SUPERUSER, Permission
+from nonebot.rule import Rule
+from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent, GuildMessageEvent
+
+from ..config import plugin_config
+
+
+def get_path(*other):
+    """获取数据文件绝对路径"""
+    if plugin_config.haruka_dir:
+        dir_path = Path(plugin_config.haruka_dir).resolve()
+    else:
+        dir_path = Path.cwd().joinpath("data")
+        # dir_path = Path.cwd().joinpath('data', 'haruka_bot')
+    return str(dir_path.joinpath(*other))
+
+
+async def handle_uid(
+    matcher: Matcher,
+    command_arg: Message = CommandArg(),
+):
+    uid = command_arg.extract_plain_text().strip()
+    if uid:
+        matcher.set_arg("uid", command_arg)
+
+
+async def uid_check(
+    matcher: Matcher,
+    uid: str = ArgPlainText("uid"),
+):
+    uid = uid.strip()
+    if not uid.isdecimal():
+        await matcher.finish("UID 必须为纯数字")
+    matcher.set_arg("uid", Message(uid))
+
+
+async def _guild_admin(bot: Bot, event: GuildMessageEvent):
+    roles = set(
+        role["role_name"]
+        for role in (
+            await bot.get_guild_member_profile(
+                guild_id=event.guild_id, user_id=event.user_id
+            )
+        )["roles"]
+    )
+    return bool(roles & set(plugin_config.haruka_guild_admin_roles))
+
+
+GUILD_ADMIN: Permission = Permission(_guild_admin)
+
+
+async def permission_check(
+    bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent, GuildMessageEvent]
+):
+    from ..database import DB as db
+
+    if isinstance(event, PrivateMessageEvent):
+        if event.sub_type == "group":  # 不处理群临时会话
+            raise FinishedException
+        return
+    if isinstance(event, GroupMessageEvent):
+        if not await db.get_group_admin(event.group_id):
+            return
+        if await (GROUP_ADMIN | GROUP_OWNER | SUPERUSER)(bot, event):
+            return
+    elif isinstance(event, GuildMessageEvent):
+        if not await db.get_guild_admin(event.guild_id, event.channel_id):
+            return
+        if await (GUILD_ADMIN | SUPERUSER)(bot, event):
+            return
+    await bot.send(event, "权限不足，目前只有管理员才能使用")
+    raise FinishedException
+
+
+async def group_only(
+    matcher: Matcher, event: PrivateMessageEvent, command: str = RawCommand()
+):
+    await matcher.finish(f"只有群里才能{command}")
+
+
+def to_me():
+    if plugin_config.haruka_to_me:
+        from nonebot.rule import to_me
+
+        return to_me()
+
+    async def _to_me() -> bool:
+        return True
+
+    return Rule(_to_me)
+
+
+async def safe_send(bot_id, send_type, type_id, message, at=False):
+    """发送出现错误时, 尝试重新发送, 并捕获异常且不会中断运行"""
+
+    async def _safe_send(bot, send_type, type_id, message):
+        if send_type == "guild":
+            from ..database import DB as db
+
+            guild = await db.get_guild(id=type_id)
+            assert guild
+            result = await bot.send_guild_channel_msg(
+                guild_id=guild.guild_id,
+                channel_id=guild.channel_id,
+                message=message,
+            )
+        else:
+            result = await bot.call_api(
+                "send_" + send_type + "_msg",
+                **{
+                    "message": message,
+                    "user_id" if send_type == "private" else "group_id": type_id,
+                },
+            )
+        return result
+
+    bots = nonebot.get_bots()
+    bot = bots.get(str(bot_id))
+    if bot is None:
+        logger.error(f"推送失败，Bot（{bot_id}）未连接，尝试使用其他 Bot 推送")
+        for bot_id, bot in bots.items():
+            if at and (
+                send_type == "guild"
+                or (await bot.get_group_at_all_remain(group_id=type_id))["can_at_all"]
+            ):
+                message = MessageSegment.at("all") + message
+            try:
+                result = await _safe_send(bot, send_type, type_id, message)
+                logger.info(f"尝试使用 Bot（{bot_id}）推送成功")
+                return result
+            except Exception:
+                continue
+        logger.error("尝试失败，所有 Bot 均无法推送")
+        return
+
+    if at and (
+        send_type == "guild"
+        or (await bot.get_group_at_all_remain(group_id=type_id))["can_at_all"]
+    ):
+        message = MessageSegment.at("all") + message
+
+    try:
+        return await _safe_send(bot, send_type, type_id, message)
+    except ActionFailed as e:
+        if e.info["msg"] == "GROUP_NOT_FOUND":
+            from ..database import DB as db
+
+            await db.delete_sub_list(type="group", type_id=type_id)
+            await db.delete_group(id=type_id)
+            logger.error(f"推送失败，群（{type_id}）不存在，已自动清理群订阅列表")
+        elif e.info["msg"] == "CHANNEL_NOT_FOUND":
+            from ..database import DB as db
+
+            guild = await db.get_guild(id=type_id)
+            assert guild
+            await db.delete_sub_list(type="guild", type_id=type_id)
+            await db.delete_guild(id=type_id)
+            logger.error(f"推送失败，频道（{guild.guild_id}|{guild.channel_id}）不存在，已自动清理频道订阅列表")
+        elif e.info["msg"] == "SEND_MSG_API_ERROR":
+            url = "https://haruka-bot.sk415.icu/usage/faq.html#机器人不发消息也没反应"
+            logger.error(f"推送失败，账号可能被风控（{url}），错误信息：{e.info}")
+        else:
+            logger.error(f"推送失败，未知错误，错误信息：{e.info}")
+    except NetworkError as e:
+        logger.error(f"推送失败，请检查网络连接，错误信息：{e.msg}")
+
+
+async def get_type_id(event: Union[MessageEvent, ChannelDestroyedNoticeEvent]):
+    if isinstance(event, GuildMessageEvent) or isinstance(
+        event, ChannelDestroyedNoticeEvent
+    ):
+        from ..database import DB as db
+
+        return await db.get_guild_type_id(event.guild_id, event.channel_id)
+    return event.group_id if isinstance(event, GroupMessageEvent) else event.user_id
+
+
+def check_proxy():
+    """检查代理是否有效"""
+    if plugin_config.haruka_proxy:
+        logger.info("检查代理是否有效")
+        try:
+            httpx.get(
+                "https://icanhazip.com/",
+                proxies={"all://": plugin_config.haruka_proxy},
+                timeout=2,
+            )
+        except Exception:
+            raise RuntimeError("加载失败，代理无法连接，请检查 HARUKA_PROXY 后重试")
+
+
+def on_startup():
+    """安装依赖并检查当前环境是否满足运行条件"""
+    if plugin_config.fastapi_reload and sys.platform == "win32":
+        raise ImportError("加载失败，Windows 必须设置 FASTAPI_RELOAD=false 才能正常运行 HarukaBot")
+    try:  # 如果开启 realod 只在第一次运行
+        asyncio.get_running_loop()
+    except RuntimeError:
+        from .browser import check_playwright_env, install
+
+        check_proxy()
+        install()
+        asyncio.get_event_loop().run_until_complete(check_playwright_env())
+        # 创建数据存储目录
+        if not Path(get_path()).is_dir():
+            Path(get_path()).mkdir(parents=True)
+
+
+def on_command(cmd, *args, **kwargs):
+    return _on_command(plugin_config.haruka_command_prefix + cmd, *args, **kwargs)
+
+
+PROXIES = {"all://": plugin_config.haruka_proxy}
+
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler  # noqa
+
+from .browser import get_dynamic_screenshot  # noqa
```

### Comparing `haruka-bot-1.5.4/haruka_bot/utils/browser.py` & `haruka-bot-1.6.0/haruka_bot/utils/browser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,202 +1,206 @@
-import asyncio
-import os
-import re
-import sys
-from pathlib import Path
-from typing import Optional
-
-from nonebot.log import logger
-from playwright.__main__ import main
-from playwright.async_api import Browser, async_playwright
-
-from ..config import plugin_config
-from .fonts_provider import fill_font
-
-_browser: Optional[Browser] = None
-mobile_js = Path(__file__).parent.joinpath("mobile.js")
-
-
-async def init_browser(proxy=plugin_config.haruka_proxy, **kwargs) -> Browser:
-    if proxy:
-        kwargs["proxy"] = {"server": proxy}
-    global _browser
-    p = await async_playwright().start()
-    _browser = await p.chromium.launch(**kwargs)
-    return _browser
-
-
-async def get_browser() -> Browser:
-    global _browser
-    if _browser is None or not _browser.is_connected():
-        _browser = await init_browser()
-    return _browser
-
-
-async def get_dynamic_screenshot(
-    dynamic_id, style=plugin_config.haruka_screenshot_style
-):
-    """获取动态截图"""
-    if style.lower() == "mobile":
-        return await get_dynamic_screenshot_mobile(dynamic_id)
-    else:
-        return await get_dynamic_screenshot_pc(dynamic_id)
-
-
-async def get_dynamic_screenshot_mobile(dynamic_id):
-    """移动端动态截图"""
-    url = f"https://m.bilibili.com/dynamic/{dynamic_id}"
-    browser = await get_browser()
-    page = await browser.new_page(
-        device_scale_factor=2,
-        user_agent=(
-            "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
-            "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
-        ),
-        viewport={"width": 460, "height": 780},
-    )
-    try:
-        await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
-        await page.goto(
-            url,
-            wait_until="networkidle",
-            timeout=plugin_config.haruka_dynamic_timeout * 1000,
-        )
-        # 动态被删除或者进审核了
-        if page.url == "https://m.bilibili.com/404":
-            return None
-        # await page.add_script_tag(
-        #     content=
-        #     # 去除打开app按钮
-        #     "document.getElementsByClassName('m-dynamic-float-openapp').forEach(v=>v.remove());"
-        #     # 去除关注按钮
-        #     "document.getElementsByClassName('dyn-header__following').forEach(v=>v.remove());"
-        #     # 修复字体与换行问题
-        #     "const dyn=document.getElementsByClassName('dyn-card')[0];"
-        #     "dyn.style.fontFamily='Noto Sans CJK SC, sans-serif';"
-        #     "dyn.style.overflowWrap='break-word'"
-        # )
-        await page.add_script_tag(path=mobile_js)
-
-        await page.evaluate(
-            f'setFont("{plugin_config.haruka_dynamic_font}", '
-            f'"{plugin_config.haruka_dynamic_font_source}")'
-            if plugin_config.haruka_dynamic_font
-            else "setFont()"
-        )
-        await page.wait_for_function("getMobileStyle()")
-
-        await page.wait_for_load_state("networkidle")
-        await page.wait_for_load_state("domcontentloaded")
-
-        await page.wait_for_timeout(
-            200 if plugin_config.haruka_dynamic_font_source == "remote" else 50
-        )
-
-        # 判断字体是否加载完成
-        need_wait = ["imageComplete", "fontsLoaded"]
-        await asyncio.gather(*[page.wait_for_function(f"{i}()") for i in need_wait])
-
-        card = await page.query_selector(
-            ".opus-modules" if "opus" in page.url else ".dyn-card"
-        )
-        assert card
-        clip = await card.bounding_box()
-        assert clip
-        return await page.screenshot(clip=clip, full_page=True)
-    except Exception:
-        logger.exception(f"截取动态时发生错误：{url}")
-        return await page.screenshot(full_page=True)
-    finally:
-        await page.close()
-
-
-async def get_dynamic_screenshot_pc(dynamic_id):
-    """电脑端动态截图"""
-    url = f"https://t.bilibili.com/{dynamic_id}"
-    browser = await get_browser()
-    context = await browser.new_context(
-        viewport={"width": 2560, "height": 1080},
-        device_scale_factor=2,
-    )
-    await context.add_cookies(
-        [
-            {
-                "name": "hit-dyn-v2",
-                "value": "1",
-                "domain": ".bilibili.com",
-                "path": "/",
-            }
-        ]
-    )
-    page = await context.new_page()
-    try:
-        await page.goto(
-            url,
-            wait_until="networkidle",
-            timeout=plugin_config.haruka_dynamic_timeout * 1000,
-        )
-        # 动态被删除或者进审核了
-        if page.url == "https://www.bilibili.com/404":
-            return None
-        card = await page.query_selector(".card")
-        assert card
-        clip = await card.bounding_box()
-        assert clip
-        bar = await page.query_selector(".bili-dyn-action__icon")
-        assert bar
-        bar_bound = await bar.bounding_box()
-        assert bar_bound
-        clip["height"] = bar_bound["y"] - clip["y"]
-        return await page.screenshot(clip=clip, full_page=True)
-    except Exception:
-        logger.exception(f"截取动态时发生错误：{url}")
-        return await page.screenshot(full_page=True)
-    finally:
-        await context.close()
-
-
-def install():
-    """自动安装、更新 Chromium"""
-
-    def restore_env():
-        del os.environ["PLAYWRIGHT_DOWNLOAD_HOST"]
-        if plugin_config.haruka_proxy:
-            del os.environ["HTTPS_PROXY"]
-        if original_proxy is not None:
-            os.environ["HTTPS_PROXY"] = original_proxy
-
-    logger.info("检查 Chromium 更新")
-    sys.argv = ["", "install", "chromium"]
-    original_proxy = os.environ.get("HTTPS_PROXY")
-    if plugin_config.haruka_proxy:
-        os.environ["HTTPS_PROXY"] = plugin_config.haruka_proxy
-    os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = "https://npmmirror.com/mirrors/playwright/"
-    success = False
-    try:
-        main()
-    except SystemExit as e:
-        if e.code == 0:
-            success = True
-    if not success:
-        logger.info("Chromium 更新失败，尝试从原始仓库下载，速度较慢")
-        os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = ""
-        try:
-            main()
-        except SystemExit as e:
-            if e.code != 0:
-                restore_env()
-                raise RuntimeError("未知错误，Chromium 下载失败")
-    restore_env()
-
-
-async def check_playwright_env():
-    """检查 Playwright 依赖"""
-    logger.info("检查 Playwright 依赖")
-    try:
-        async with async_playwright() as p:
-            await p.chromium.launch()
-    except Exception:
-        raise ImportError(
-            "加载失败，Playwright 依赖不全，"
-            "解决方法：https://haruka-bot.sk415.icu/faq.html#playwright-依赖不全"
-        )
+import asyncio
+import os
+import re
+import sys
+from pathlib import Path
+from typing import Optional
+
+from nonebot.log import logger
+from playwright.__main__ import main
+from playwright.async_api import Browser, async_playwright
+
+from ..config import plugin_config
+from .fonts_provider import fill_font
+from .captcha import resolve_captcha
+
+_browser: Optional[Browser] = None
+mobile_js = Path(__file__).parent.joinpath("mobile.js")
+
+
+async def init_browser(proxy=plugin_config.haruka_proxy, **kwargs) -> Browser:
+    if proxy:
+        kwargs["proxy"] = {"server": proxy}
+    global _browser
+    p = await async_playwright().start()
+    _browser = await p.chromium.launch(**kwargs)
+    return _browser
+
+
+async def get_browser() -> Browser:
+    global _browser
+    if _browser is None or not _browser.is_connected():
+        _browser = await init_browser()
+    return _browser
+
+
+async def get_dynamic_screenshot(
+    dynamic_id, style=plugin_config.haruka_screenshot_style
+):
+    """获取动态截图"""
+    if style.lower() == "mobile":
+        return await get_dynamic_screenshot_mobile(dynamic_id)
+    else:
+        return await get_dynamic_screenshot_pc(dynamic_id)
+
+
+async def get_dynamic_screenshot_mobile(dynamic_id):
+    """移动端动态截图"""
+    url = f"https://m.bilibili.com/dynamic/{dynamic_id}"
+    browser = await get_browser()
+    page = await browser.new_page(
+        device_scale_factor=2,
+        user_agent=(
+            "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
+            "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
+        ),
+        viewport={"width": 460, "height": 780},
+    )
+    try:
+        await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
+        if plugin_config.haruka_captcha_address:
+            page = await resolve_captcha(url,page)
+        else:
+            await page.goto(
+                url,
+                wait_until="networkidle",
+                timeout=plugin_config.haruka_dynamic_timeout * 1000,
+            )
+        # 动态被删除或者进审核了
+        if page.url == "https://m.bilibili.com/404":
+            return None
+        # await page.add_script_tag(
+        #     content=
+        #     # 去除打开app按钮
+        #     "document.getElementsByClassName('m-dynamic-float-openapp').forEach(v=>v.remove());"
+        #     # 去除关注按钮
+        #     "document.getElementsByClassName('dyn-header__following').forEach(v=>v.remove());"
+        #     # 修复字体与换行问题
+        #     "const dyn=document.getElementsByClassName('dyn-card')[0];"
+        #     "dyn.style.fontFamily='Noto Sans CJK SC, sans-serif';"
+        #     "dyn.style.overflowWrap='break-word'"
+        # )
+        await page.add_script_tag(path=mobile_js)
+
+        await page.evaluate(
+            f'setFont("{plugin_config.haruka_dynamic_font}", '
+            f'"{plugin_config.haruka_dynamic_font_source}")'
+            if plugin_config.haruka_dynamic_font
+            else "setFont()"
+        )
+        await page.wait_for_function("getMobileStyle()")
+
+        await page.wait_for_load_state("networkidle")
+        await page.wait_for_load_state("domcontentloaded")
+
+        await page.wait_for_timeout(
+            200 if plugin_config.haruka_dynamic_font_source == "remote" else 50
+        )
+
+        # 判断字体是否加载完成
+        need_wait = ["imageComplete", "fontsLoaded"]
+        await asyncio.gather(*[page.wait_for_function(f"{i}()") for i in need_wait])
+
+        card = await page.query_selector(
+            ".opus-modules" if "opus" in page.url else ".dyn-card"
+        )
+        assert card
+        clip = await card.bounding_box()
+        assert clip
+        return await page.screenshot(clip=clip, full_page=True)
+    except Exception:
+        logger.exception(f"截取动态时发生错误：{url}")
+        return await page.screenshot(full_page=True)
+    finally:
+        await page.close()
+
+
+async def get_dynamic_screenshot_pc(dynamic_id):
+    """电脑端动态截图"""
+    url = f"https://t.bilibili.com/{dynamic_id}"
+    browser = await get_browser()
+    context = await browser.new_context(
+        viewport={"width": 2560, "height": 1080},
+        device_scale_factor=2,
+    )
+    await context.add_cookies(
+        [
+            {
+                "name": "hit-dyn-v2",
+                "value": "1",
+                "domain": ".bilibili.com",
+                "path": "/",
+            }
+        ]
+    )
+    page = await context.new_page()
+    try:
+        await page.goto(
+            url,
+            wait_until="networkidle",
+            timeout=plugin_config.haruka_dynamic_timeout * 1000,
+        )
+        # 动态被删除或者进审核了
+        if page.url == "https://www.bilibili.com/404":
+            return None
+        card = await page.query_selector(".card")
+        assert card
+        clip = await card.bounding_box()
+        assert clip
+        bar = await page.query_selector(".bili-dyn-action__icon")
+        assert bar
+        bar_bound = await bar.bounding_box()
+        assert bar_bound
+        clip["height"] = bar_bound["y"] - clip["y"]
+        return await page.screenshot(clip=clip, full_page=True)
+    except Exception:
+        logger.exception(f"截取动态时发生错误：{url}")
+        return await page.screenshot(full_page=True)
+    finally:
+        await context.close()
+
+
+def install():
+    """自动安装、更新 Chromium"""
+
+    def restore_env():
+        del os.environ["PLAYWRIGHT_DOWNLOAD_HOST"]
+        if plugin_config.haruka_proxy:
+            del os.environ["HTTPS_PROXY"]
+        if original_proxy is not None:
+            os.environ["HTTPS_PROXY"] = original_proxy
+
+    logger.info("检查 Chromium 更新")
+    sys.argv = ["", "install", "chromium"]
+    original_proxy = os.environ.get("HTTPS_PROXY")
+    if plugin_config.haruka_proxy:
+        os.environ["HTTPS_PROXY"] = plugin_config.haruka_proxy
+    os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = "https://npmmirror.com/mirrors/playwright/"
+    success = False
+    try:
+        main()
+    except SystemExit as e:
+        if e.code == 0:
+            success = True
+    if not success:
+        logger.info("Chromium 更新失败，尝试从原始仓库下载，速度较慢")
+        os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = ""
+        try:
+            main()
+        except SystemExit as e:
+            if e.code != 0:
+                restore_env()
+                raise RuntimeError("未知错误，Chromium 下载失败")
+    restore_env()
+
+
+async def check_playwright_env():
+    """检查 Playwright 依赖"""
+    logger.info("检查 Playwright 依赖")
+    try:
+        async with async_playwright() as p:
+            await p.chromium.launch()
+    except Exception:
+        raise ImportError(
+            "加载失败，Playwright 依赖不全，"
+            "解决方法：https://haruka-bot.sk415.icu/faq.html#playwright-依赖不全"
+        )
```

### Comparing `haruka-bot-1.5.4/haruka_bot/utils/fonts_provider.py` & `haruka-bot-1.6.0/haruka_bot/utils/fonts_provider.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from playwright.async_api import Request, Route
-from yarl import URL
-from loguru import logger
-
-from pathlib import Path
-
-font_path = Path("font")
-
-font_mime_map = {
-    "collection": "font/collection",
-    "otf": "font/otf",
-    "sfnt": "font/sfnt",
-    "ttf": "font/ttf",
-    "woff": "font/woff",
-    "woff2": "font/woff2",
-}
-
-
-async def fill_font(route: Route, request: Request):
-    url = URL(request.url)
-    if font_path.joinpath(url.name).exists():
-        logger.debug(f"Font {url.name} found in local")
-        await route.fulfill(
-            path=font_path.joinpath(url.name),
-            content_type=font_mime_map.get(url.suffix, None),
-        )
-        return
-    await route.fallback()
+from playwright.async_api import Request, Route
+from yarl import URL
+from loguru import logger
+
+from pathlib import Path
+
+font_path = Path("font")
+
+font_mime_map = {
+    "collection": "font/collection",
+    "otf": "font/otf",
+    "sfnt": "font/sfnt",
+    "ttf": "font/ttf",
+    "woff": "font/woff",
+    "woff2": "font/woff2",
+}
+
+
+async def fill_font(route: Route, request: Request):
+    url = URL(request.url)
+    if font_path.joinpath(url.name).exists():
+        logger.debug(f"Font {url.name} found in local")
+        await route.fulfill(
+            path=font_path.joinpath(url.name),
+            content_type=font_mime_map.get(url.suffix, None),
+        )
+        return
+    await route.fallback()
```

### Comparing `haruka-bot-1.5.4/haruka_bot/utils/mobile.js` & `haruka-bot-1.6.0/haruka_bot/utils/mobile.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,195 +1,195 @@
-/*
- * @Author: KBD
- * @Date: 2022-12-26 13:45:30
- * @LastEditors: KBD
- * @LastEditTime: 2023-01-13 01:35:34
- * @Description: 用于初始化手机动态页面的样式以及图片大小
- */
-async function getMobileStyle() {
-    // 删除 dom 的对象, 可以自行添加 ( className 需要增加 '.' 为前缀, id 需要增加 '#' 为前缀)
-    const deleteDoms = {
-        // 关注 dom
-        followDoms: [".dyn-header__following", ".easy-follow-btn"],
-        // 分享 dom
-        shareDoms: [".dyn-share"],
-        // 打开程序 dom
-        openAppBtnDoms: [".dynamic-float-btn", ".float-openapp"],
-        // 导航 dom
-        navDoms: [".m-navbar", ".opus-nav"],
-        // 获取更多 dom
-        readMoreDoms: [".opus-read-more"],
-        // 全屏弹出 Dom
-        openAppDialogDoms: [".openapp-dialog"],
-        // 评论区 dom
-        commentsDoms: [".v-switcher"],
-    }
-
-    // 遍历对象的值, 并将多数组扁平化, 再遍历进行删除操作
-    Object.values(deleteDoms).flat(1).forEach(domTag => {
-        const deleteDom = document.querySelector(domTag);
-        deleteDom && deleteDom.remove();
-    })
-
-    // 新版动态需要移除对应 class 达到跳过点击事件, 解除隐藏的目的 
-    const contentDom = document.querySelector(".opus-module-content");
-    contentDom && contentDom.classList.remove("limit");
-
-    // // 新版动态需要给 bm-pics-block 的父级元素设置 flex 以及 column
-    // const newContainerDom = document.querySelector(".bm-pics-block")?.parentElement;
-    // if (newContainerDom) {
-    //     // 设置为 flex
-    //     newContainerDom.style.display = "flex";
-    //     // 设置为竖向排列
-    //     newContainerDom.style.flexDirection = "column";
-    //     // flex - 垂直居中
-    //     newContainerDom.style.justifyContent = "center";
-    //     // flex - 水平居中
-    //     newContainerDom.style.alignItems = "center";
-    // }
-
-    // 设置 mopus 的 paddingTop 为 0
-    const mOpusDom = document.querySelector(".m-opus");
-    if (mOpusDom) {
-        mOpusDom.style.paddingTop = "0";
-        mOpusDom.style.minHeight = "0";
-    }
-
-    // 删除老版动态 .dyn-card 上的字体设置
-    const dynCardDom = document.querySelector(".dyn-card");
-    if (dynCardDom) {
-        dynCardDom.style.fontFamily = "unset";
-    }
-
-    // // 找到图标容器dom
-    // const containerDom = document.querySelector(".bm-pics-block__container");
-    // if (containerDom) {
-    //     // 先把默认 padding-left 置为0
-    //     containerDom.style.paddingLeft = "0";
-    //     // 先把默认 padding-right 置为0
-    //     containerDom.style.paddingRight = "0";
-    //     // 设置 flex 模式下以列形式排列
-    //     containerDom.style.flexDirection = "column";
-    //     // 设置 flex 模式下每个容器间隔15px
-    //     containerDom.style.gap = "15px";
-    //     // flex - 垂直居中
-    //     containerDom.style.justifyContent = "center";
-    //     // flex - 水平居中
-    //     containerDom.style.alignItems = "center";
-    // }
-
-    // 获取图片容器的所有 dom
-    const imageItemDoms = document.querySelectorAll(".bm-pics-block__item");
-
-    // 异步遍历图片 dom
-    Array.from(imageItemDoms).map(async (item) => {
-        // // 获取屏幕比例的 90% 宽度
-        // const clientWidth = window.innerWidth * 0.9;
-        // // 先把默认 margin 置为 0
-        // item.style.margin = "0";
-        // // 宽度默认撑满屏幕宽度 90%;
-        // item.style.width = `${clientWidth}px`;
-        // 获取原app中图片的src
-        const imgSrc = item.firstChild.src;
-        // 判断是否有 @ 符
-        const imgSrcAtIndex = imgSrc.indexOf("@");
-        // 将所有图片转换为 .webp 格式节省加载速度, 并返回给原来的 image 标签
-        item.firstChild.src = imgSrcAtIndex !== -1 ? imgSrc.slice(0, imgSrcAtIndex + 1) + ".webp" : imgSrc;
-        // // 设置自动高度
-        // item.style.height = "auto";
-    })
-}
-
-
-function setFont(font = "", fontSource = "local") {
-    // TODO: 未来考虑添加本地离线字体
-    // 自行添加在线字体(字体的优先度将按照顺序执行)
-    const needLoadFontList = [{
-        fontUrl: "https://cdn.jsdelivr.net/gh/irozhi/HarmonyOS-Sans/HarmonyOS_Sans_SC/HarmonyOS_Sans_SC_Medium.woff2",
-        fontFamily: "HarmonyOS_Medium_woff2",
-    }];
-    const emojiFontList = ["Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"];
-
-    if (font) {
-        // 如果传入了字体名, 则将其添加到字体列表首位
-        if (fontSource === "local") {
-            needLoadFontList.unshift({
-                fontUrl: `https://fonts.bbot/${font}`,
-                fontFamily: "BBot_Custom_Font",
-            });
-        } else if (fontSource === "remote") {
-            needLoadFontList.unshift({
-                fontUrl: font,
-                fontFamily: "BBot_Custom_Font",
-            });
-        }
-    }
-
-    // 字体按需加载方法
-    (() => {
-        const code = needLoadFontList.reduce((defaultString, fontObject) => {
-            return defaultString + `@font-face { font-family: ${fontObject.fontFamily};src: url('${fontObject.fontUrl}'); }`;
-        }, "");
-        const style = document.createElement("style");
-        style.rel = "stylesheet";
-        style.appendChild(document.createTextNode(code));
-        const head = document.getElementsByTagName("head")[0];
-        head.appendChild(style);
-    })();
-
-    // 将字体样式设置到 div#app 上
-    const appDom = document.querySelector("#app");
-    const emojiFont = emojiFontList.join(",");
-    if (appDom) {
-        // 动态加字体, 并给与默认值 sans-serif
-        if (fontSource === "system") {
-            appDom.style.fontFamily = font + "," + emojiFont + ",sans-serif";
-        } else {
-            const needLoadFont = needLoadFontList.reduce((defaultString, fontObject) => defaultString + fontObject.fontFamily + ",", "");
-            appDom.style.fontFamily = needLoadFont + emojiFont + ",sans-serif";
-        };
-        appDom.style.overflowWrap = "break-word";
-    }
-
-    return font;
-}
-
-
-async function imageComplete() {
-    // 异步渲染已经加载的图片地址, 如果已经缓存则会立即返回 true
-    const loadImageAsync = (url) => {
-        return new Promise((resolve, reject) => {
-            const image = new Image();
-            image.src = url;
-
-            image.onload = () => {
-                resolve(image.complete) // 理应为 true
-            }
-
-            image.onerror = () => {
-                reject(false);
-            }
-        })
-    }
-
-    // 获取图片容器的所有 dom
-    const imageItemDoms = document.querySelectorAll(".bm-pics-block__item");
-
-    // 异步遍历图片并等待
-    const imageItemStatusArray = await Promise.all(Array.from(imageItemDoms).map((item) => {
-        return loadImageAsync(item.firstChild.src);
-    }))
-
-    // 通过遍历图片加载状态, 如果有一个图片加载失败, 均为 false
-    return imageItemStatusArray.reduce((p, c) => {
-        return p && c;
-    }, true)
-}
-
-function fontsLoaded() {
-    // 判断字体是否都加载完成
-    return document.fonts.status === "loaded";
-}
-
-window.onload = () => {
-    getMobileStyle();
+/*
+ * @Author: KBD
+ * @Date: 2022-12-26 13:45:30
+ * @LastEditors: KBD
+ * @LastEditTime: 2023-01-13 01:35:34
+ * @Description: 用于初始化手机动态页面的样式以及图片大小
+ */
+async function getMobileStyle() {
+    // 删除 dom 的对象, 可以自行添加 ( className 需要增加 '.' 为前缀, id 需要增加 '#' 为前缀)
+    const deleteDoms = {
+        // 关注 dom
+        followDoms: [".dyn-header__following", ".easy-follow-btn"],
+        // 分享 dom
+        shareDoms: [".dyn-share"],
+        // 打开程序 dom
+        openAppBtnDoms: [".dynamic-float-btn", ".float-openapp"],
+        // 导航 dom
+        navDoms: [".m-navbar", ".opus-nav"],
+        // 获取更多 dom
+        readMoreDoms: [".opus-read-more"],
+        // 全屏弹出 Dom
+        openAppDialogDoms: [".openapp-dialog"],
+        // 评论区 dom
+        commentsDoms: [".v-switcher"],
+    }
+
+    // 遍历对象的值, 并将多数组扁平化, 再遍历进行删除操作
+    Object.values(deleteDoms).flat(1).forEach(domTag => {
+        const deleteDom = document.querySelector(domTag);
+        deleteDom && deleteDom.remove();
+    })
+
+    // 新版动态需要移除对应 class 达到跳过点击事件, 解除隐藏的目的 
+    const contentDom = document.querySelector(".opus-module-content");
+    contentDom && contentDom.classList.remove("limit");
+
+    // // 新版动态需要给 bm-pics-block 的父级元素设置 flex 以及 column
+    // const newContainerDom = document.querySelector(".bm-pics-block")?.parentElement;
+    // if (newContainerDom) {
+    //     // 设置为 flex
+    //     newContainerDom.style.display = "flex";
+    //     // 设置为竖向排列
+    //     newContainerDom.style.flexDirection = "column";
+    //     // flex - 垂直居中
+    //     newContainerDom.style.justifyContent = "center";
+    //     // flex - 水平居中
+    //     newContainerDom.style.alignItems = "center";
+    // }
+
+    // 设置 mopus 的 paddingTop 为 0
+    const mOpusDom = document.querySelector(".m-opus");
+    if (mOpusDom) {
+        mOpusDom.style.paddingTop = "0";
+        mOpusDom.style.minHeight = "0";
+    }
+
+    // 删除老版动态 .dyn-card 上的字体设置
+    const dynCardDom = document.querySelector(".dyn-card");
+    if (dynCardDom) {
+        dynCardDom.style.fontFamily = "unset";
+    }
+
+    // // 找到图标容器dom
+    // const containerDom = document.querySelector(".bm-pics-block__container");
+    // if (containerDom) {
+    //     // 先把默认 padding-left 置为0
+    //     containerDom.style.paddingLeft = "0";
+    //     // 先把默认 padding-right 置为0
+    //     containerDom.style.paddingRight = "0";
+    //     // 设置 flex 模式下以列形式排列
+    //     containerDom.style.flexDirection = "column";
+    //     // 设置 flex 模式下每个容器间隔15px
+    //     containerDom.style.gap = "15px";
+    //     // flex - 垂直居中
+    //     containerDom.style.justifyContent = "center";
+    //     // flex - 水平居中
+    //     containerDom.style.alignItems = "center";
+    // }
+
+    // 获取图片容器的所有 dom
+    const imageItemDoms = document.querySelectorAll(".bm-pics-block__item");
+
+    // 异步遍历图片 dom
+    Array.from(imageItemDoms).map(async (item) => {
+        // // 获取屏幕比例的 90% 宽度
+        // const clientWidth = window.innerWidth * 0.9;
+        // // 先把默认 margin 置为 0
+        // item.style.margin = "0";
+        // // 宽度默认撑满屏幕宽度 90%;
+        // item.style.width = `${clientWidth}px`;
+        // 获取原app中图片的src
+        const imgSrc = item.firstChild.src;
+        // 判断是否有 @ 符
+        const imgSrcAtIndex = imgSrc.indexOf("@");
+        // 将所有图片转换为 .webp 格式节省加载速度, 并返回给原来的 image 标签
+        item.firstChild.src = imgSrcAtIndex !== -1 ? imgSrc.slice(0, imgSrcAtIndex + 1) + ".webp" : imgSrc;
+        // // 设置自动高度
+        // item.style.height = "auto";
+    })
+}
+
+
+function setFont(font = "", fontSource = "local") {
+    // TODO: 未来考虑添加本地离线字体
+    // 自行添加在线字体(字体的优先度将按照顺序执行)
+    const needLoadFontList = [{
+        fontUrl: "https://cdn.jsdelivr.net/gh/irozhi/HarmonyOS-Sans/HarmonyOS_Sans_SC/HarmonyOS_Sans_SC_Medium.woff2",
+        fontFamily: "HarmonyOS_Medium_woff2",
+    }];
+    const emojiFontList = ["Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"];
+
+    if (font) {
+        // 如果传入了字体名, 则将其添加到字体列表首位
+        if (fontSource === "local") {
+            needLoadFontList.unshift({
+                fontUrl: `https://fonts.bbot/${font}`,
+                fontFamily: "BBot_Custom_Font",
+            });
+        } else if (fontSource === "remote") {
+            needLoadFontList.unshift({
+                fontUrl: font,
+                fontFamily: "BBot_Custom_Font",
+            });
+        }
+    }
+
+    // 字体按需加载方法
+    (() => {
+        const code = needLoadFontList.reduce((defaultString, fontObject) => {
+            return defaultString + `@font-face { font-family: ${fontObject.fontFamily};src: url('${fontObject.fontUrl}'); }`;
+        }, "");
+        const style = document.createElement("style");
+        style.rel = "stylesheet";
+        style.appendChild(document.createTextNode(code));
+        const head = document.getElementsByTagName("head")[0];
+        head.appendChild(style);
+    })();
+
+    // 将字体样式设置到 div#app 上
+    const appDom = document.querySelector("#app");
+    const emojiFont = emojiFontList.join(",");
+    if (appDom) {
+        // 动态加字体, 并给与默认值 sans-serif
+        if (fontSource === "system") {
+            appDom.style.fontFamily = font + "," + emojiFont + ",sans-serif";
+        } else {
+            const needLoadFont = needLoadFontList.reduce((defaultString, fontObject) => defaultString + fontObject.fontFamily + ",", "");
+            appDom.style.fontFamily = needLoadFont + emojiFont + ",sans-serif";
+        };
+        appDom.style.overflowWrap = "break-word";
+    }
+
+    return font;
+}
+
+
+async function imageComplete() {
+    // 异步渲染已经加载的图片地址, 如果已经缓存则会立即返回 true
+    const loadImageAsync = (url) => {
+        return new Promise((resolve, reject) => {
+            const image = new Image();
+            image.src = url;
+
+            image.onload = () => {
+                resolve(image.complete) // 理应为 true
+            }
+
+            image.onerror = () => {
+                reject(false);
+            }
+        })
+    }
+
+    // 获取图片容器的所有 dom
+    const imageItemDoms = document.querySelectorAll(".bm-pics-block__item");
+
+    // 异步遍历图片并等待
+    const imageItemStatusArray = await Promise.all(Array.from(imageItemDoms).map((item) => {
+        return loadImageAsync(item.firstChild.src);
+    }))
+
+    // 通过遍历图片加载状态, 如果有一个图片加载失败, 均为 false
+    return imageItemStatusArray.reduce((p, c) => {
+        return p && c;
+    }, true)
+}
+
+function fontsLoaded() {
+    // 判断字体是否都加载完成
+    return document.fonts.status === "loaded";
+}
+
+window.onload = () => {
+    getMobileStyle();
 }
```

### Comparing `haruka-bot-1.5.4/LICENSE` & `haruka-bot-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.4/pyproject.toml` & `haruka-bot-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bilibili",
     "bot",
 ]
-version = "1.5.4"
+version = "1.6.0"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/SK-415/HarukaBot"
 repository = "https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot"
```

### Comparing `haruka-bot-1.5.4/README.md` & `haruka-bot-1.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-[![HarukaBot](https://socialify.git.ci/SK-415/HarukaBot/image?description=1&font=Source%20Code%20Pro&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FSK-415%2FHarukaBot%2Fmaster%2Fdocs%2F.vuepress%2Fpublic%2Flogo.png&owner=1&pattern=Charlie%20Brown&stargazers=1&theme=Dark)](https://haruka-bot.sk415.icu/)
-
-# [HarukaBot](https://haruka-bot.sk415.icu)——优雅的 B 站推送 QQ 机器人
-
-名称来源：[@白神遥Haruka](https://space.bilibili.com/477332594)
-
-Logo 画师：[@Ratto](https://space.bilibili.com/23242907)
-
-[![VERSION](https://img.shields.io/pypi/v/haruka-bot)](https://haruka-bot.sk415.icu/about/CHANGELOG.html)
-[![qq group](https://img.shields.io/badge/QQ%E7%BE%A4-629574472-orange)](https://jq.qq.com/?_wv=1027&k=sHPbCRAd)
-[![time tracker](https://wakatime.com/badge/github/SK-415/HarukaBot.svg)](https://wakatime.com/badge/github/SK-415/HarukaBot)
-
-## 简介
-
-一款将哔哩哔哩 UP 主的直播与动态信息推送至 QQ 的机器人。基于 [NoneBot2](https://github.com/nonebot/nonebot2) 开发，前身为 [dd-bot](https://github.com/SK-415/dd-bot) 。
-
-## 特色功能
-
-HarukaBot 针对不同的推送场景（粉丝群、娱乐群、直播通知群），提供了个性化设置：
-
-- 自定义推送内容，每位 UP 主可限制仅动态、仅直播。
-- 群内开启权限限制，仅管理员以上可以使用机器人。
-- 指定推送内容@全体成员，次数用光自动忽略。
-- 同时连接多个 QQ 号，避免@全体成员次数不够。
-
-## [文档（点击查看）](https://haruka-bot.sk415.icu)
-
-## 部分功能展示
-
-![demo](/docs/.vuepress/public/demo.png)
-
-## 特别感谢
-
-- [@mnixry](https://github.com/mnixry)：感谢混淆佬为本项目提供的**技♂术指导**。
-- [@wosiwq](https://github.com/wosiwq)：感谢 W 桑撰写的「小小白白话文」。
-- [NoneBot2](https://github.com/nonebot/nonebot2)：HarukaBot 使用的开发框架。
-- [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
-- [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect)：非常详细的 B 站 API 文档。
-- [bilibili_api](https://github.com/Passkou/bilibili_api)：Python 实现的 B 站 API 库。
-- [HarukaBot_Guild_Patch](https://github.com/17TheWord/HarukaBot_Guild_Patch) 可以让HarukaBot适用于频道的补丁。（已合入 HarukaBot）
-
-## 支持与贡献
-
-觉得好用可以给这个项目点个 Star 或者去 [爱发电](https://afdian.net/@HarukaBot) 投喂我。
-
-有意见或者建议也欢迎提交 [Issues](https://github.com/SK-415/HarukaBot/issues) 和 [Pull requests](https://github.com/SK-415/HarukaBot/pulls)。
-
-## 许可证
-本项目使用 [GNU AGPLv3](https://choosealicense.com/licenses/agpl-3.0/) 作为开源许可证。
+[![HarukaBot](https://socialify.git.ci/SK-415/HarukaBot/image?description=1&font=Source%20Code%20Pro&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FSK-415%2FHarukaBot%2Fmaster%2Fdocs%2F.vuepress%2Fpublic%2Flogo.png&owner=1&pattern=Charlie%20Brown&stargazers=1&theme=Dark)](https://haruka-bot.sk415.icu/)
+
+# [HarukaBot](https://haruka-bot.sk415.icu)——优雅的 B 站推送 QQ 机器人
+
+名称来源：[@白神遥Haruka](https://space.bilibili.com/477332594)
+
+Logo 画师：[@Ratto](https://space.bilibili.com/23242907)
+
+[![VERSION](https://img.shields.io/pypi/v/haruka-bot)](https://haruka-bot.sk415.icu/about/CHANGELOG.html)
+[![qq group](https://img.shields.io/badge/QQ%E7%BE%A4-629574472-orange)](https://jq.qq.com/?_wv=1027&k=sHPbCRAd)
+[![time tracker](https://wakatime.com/badge/github/SK-415/HarukaBot.svg)](https://wakatime.com/badge/github/SK-415/HarukaBot)
+
+## 简介
+
+一款将哔哩哔哩 UP 主的直播与动态信息推送至 QQ 的机器人。基于 [NoneBot2](https://github.com/nonebot/nonebot2) 开发，前身为 [dd-bot](https://github.com/SK-415/dd-bot) 。
+
+## 特色功能
+
+HarukaBot 针对不同的推送场景（粉丝群、娱乐群、直播通知群），提供了个性化设置：
+
+- 自定义推送内容，每位 UP 主可限制仅动态、仅直播。
+- 群内开启权限限制，仅管理员以上可以使用机器人。
+- 指定推送内容@全体成员，次数用光自动忽略。
+- 同时连接多个 QQ 号，避免@全体成员次数不够。
+
+## [文档（点击查看）](https://haruka-bot.sk415.icu)
+
+## 部分功能展示
+
+![demo](/docs/.vuepress/public/demo.png)
+
+## 特别感谢
+
+- [@mnixry](https://github.com/mnixry)：感谢混淆佬为本项目提供的**技♂术指导**。
+- [@wosiwq](https://github.com/wosiwq)：感谢 W 桑撰写的「小小白白话文」。
+- [NoneBot2](https://github.com/nonebot/nonebot2)：HarukaBot 使用的开发框架。
+- [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
+- [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect)：非常详细的 B 站 API 文档。
+- [bilibili_api](https://github.com/Passkou/bilibili_api)：Python 实现的 B 站 API 库。
+- [HarukaBot_Guild_Patch](https://github.com/17TheWord/HarukaBot_Guild_Patch)：可以让HarukaBot适用于频道的补丁。（已合入 HarukaBot）
+
+## 支持与贡献
+
+觉得好用可以给这个项目点个 Star 或者去 [爱发电](https://afdian.net/@HarukaBot) 投喂我。
+
+有意见或者建议也欢迎提交 [Issues](https://github.com/SK-415/HarukaBot/issues) 和 [Pull requests](https://github.com/SK-415/HarukaBot/pulls)。
+
+## 许可证
+本项目使用 [GNU AGPLv3](https://choosealicense.com/licenses/agpl-3.0/) 作为开源许可证。
```

### Comparing `haruka-bot-1.5.4/PKG-INFO` & `haruka-bot-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka-bot
-Version: 1.5.4
+Version: 1.6.0
 Summary: Push dynamics and live informations from bilibili to QQ. Based on nonebot2.
 License: AGPL-3.0-or-later
 Keywords: nonebot,nonebot2,qqbot,bilibili,bot
 Author-email: SK-415 <2967923486@qq.com>
 Requires-Python: >=3.8,<4.0
 Project-URL: documentation, https://github.com/SK-415/HarukaBot#readme
 Project-URL: homepage, https://github.com/SK-415/HarukaBot
@@ -46,15 +46,15 @@
 
 - [@mnixry](https://github.com/mnixry)：感谢混淆佬为本项目提供的**技♂术指导**。
 - [@wosiwq](https://github.com/wosiwq)：感谢 W 桑撰写的「小小白白话文」。
 - [NoneBot2](https://github.com/nonebot/nonebot2)：HarukaBot 使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect)：非常详细的 B 站 API 文档。
 - [bilibili_api](https://github.com/Passkou/bilibili_api)：Python 实现的 B 站 API 库。
-- [HarukaBot_Guild_Patch](https://github.com/17TheWord/HarukaBot_Guild_Patch) 可以让HarukaBot适用于频道的补丁。（已合入 HarukaBot）
+- [HarukaBot_Guild_Patch](https://github.com/17TheWord/HarukaBot_Guild_Patch)：可以让HarukaBot适用于频道的补丁。（已合入 HarukaBot）
 
 ## 支持与贡献
 
 觉得好用可以给这个项目点个 Star 或者去 [爱发电](https://afdian.net/@HarukaBot) 投喂我。
 
 有意见或者建议也欢迎提交 [Issues](https://github.com/SK-415/HarukaBot/issues) 和 [Pull requests](https://github.com/SK-415/HarukaBot/pulls)。
```

