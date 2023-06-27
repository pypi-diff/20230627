# Comparing `tmp/nonebot_plugin_nagabus-0.2.3.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.4.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.3.tar` & `nonebot_plugin_nagabus-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.3/LICENSE
--rw-r--r--   0        0        0     1379 2023-06-19 13:37:42.959252 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1364 2023-06-19 13:36:03.851200 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-09 05:28:00.065113 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      715 2023-06-19 13:36:03.860199 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-09 05:28:24.454277 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4650 2023-06-09 06:01:06.071925 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2420 2023-06-01 06:58:40.633672 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1617 2023-06-09 05:51:28.775960 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      178 2023-06-19 13:36:03.827200 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3709 2023-06-09 06:12:20.123461 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0      436 2023-06-09 05:28:00.075631 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/errors.py
--rw-r--r--   0        0        0     3415 2023-06-09 15:01:04.190237 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1248 2023-06-09 15:00:22.460735 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    21194 2023-06-19 13:36:03.846202 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0      347 2023-06-09 05:53:37.650409 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      997 2023-06-19 13:38:34.784589 nonebot_plugin_nagabus-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.3/README.md
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1364 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-27 03:05:14.174566 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4650 2023-06-19 13:39:23.144435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     4040 2023-06-27 03:05:14.179567 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21282 2023-06-27 03:05:14.157193 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      997 2023-06-27 03:09:17.964805 nonebot_plugin_nagabus-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.4/README.md
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.4/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.3/LICENSE` & `nonebot_plugin_nagabus-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 nonebot-plugin-nagabus
 
 @Author         : ssttkkl
 @License        : AGPLv3
-@GitHub         : https://github.com/ssttkkl/nonebot-plugin-nagabus
+@GitHub         : https://github.com/bot-ssttkkl/nonebot-plugin-nagabus
 """
 
 from nonebot import require, logger
 from nonebot.plugin import PluginMetadata
 
 from .errors import ConfigError
 
@@ -28,23 +28,24 @@
 
 使用情况：
 {default_cmd_start}naga本月使用情况
 {default_cmd_start}naga上月使用情况
 
 以上命令格式中，以<>包裹的表示一个参数。
 
-详细说明：参见https://github.com/ssttkkl/nonebot-plugin-nagabus
+详细说明：参见https://github.com/bot-ssttkkl/nonebot-plugin-nagabus
 """.strip()
 
 __plugin_meta__ = PluginMetadata(
     name='NAGA公交车',
     description='为群友提供NAGA拼车服务',
     usage=__usage__,
     type="application",
-    homepage="https://github.com/ssttkkl/nonebot-plugin-nagabus",
-    config=Config
+    homepage="https://github.com/bot-ssttkkl/nonebot-plugin-nagabus",
+    config=Config,
+    supported_adapters={"~onebot.v11", "~onebot.v12", "~qqguild", "~kaiheila", "~telegram"}
 )
 
 try:
     from . import matchers
 except ConfigError as e:
     logger.exception(e)
```

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     await MessageFactory(e.message).send(reply=True)
                     await matcher.finish()
             except RateLimitedError as e:
                 if not silently:
                     await MessageFactory("已达到使用次数上限").send(reply=True)
                     await matcher.finish()
             except OrderError as e:
-                logger.warning(e)
+                logger.exception(e)
                 if not silently:
                     await MessageFactory("不知道为什么总之解析错误，请在NAGA网页端检查是否已成功解析").send(reply=True)
                     await matcher.finish()
             except InvalidGameError as e:
                 logger.warning(e)
                 if not silently:
                     await MessageFactory("牌谱链接不正确").send(reply=True)
```

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from datetime import datetime
 from io import StringIO
-from typing import Optional
+from typing import Optional, List
 
 from monthdelta import monthdelta
 from nonebot import on_command, Bot
 from nonebot_plugin_datastore.db import get_engine
 from nonebot_plugin_get_nickname import get_nickname
 from nonebot_plugin_saa import MessageFactory
 from nonebot_plugin_session import SessionIdType
 from nonebot_plugin_session.model import SessionModel
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from .interceptors.handle_error import handle_error
 from ..ac import ac
 from ..naga import naga
+from ..naga.model import NagaServiceUserStatistic
 from ..utils.tz import TZ_TOKYO
 
 statistic_srv = ac.create_subservice("statistic")
 
 
-async def naga_statistic(bot: Bot, year: int, month: int):
-    statistic = await naga.statistic(year, month)
-
+async def naga_statistic(bot: Bot, year: int, month: int, statistic: List[NagaServiceUserStatistic],
+                         rest_np: Optional[int] = None):
     total_cost_np = 0
 
     async with AsyncSession(get_engine()) as db_sess:
         with StringIO() as sio:
             for i, s in enumerate(statistic):
                 session_model: Optional[SessionModel] = await db_sess.get(SessionModel, s.customer_id)
                 session = session_model.session
@@ -33,32 +33,38 @@
                     nickname = session.get_id(SessionIdType.USER, include_bot_type=False, include_bot_id=False)
                 else:
                     nickname = await get_nickname(session, bot)
                 sio.write(f"#{i + 1} {nickname}: {s.cost_np}NP\n")
 
                 total_cost_np += s.cost_np
 
-            msg = (f"{year}年{month}月共使用{total_cost_np}NP\n\n" + sio.getvalue()).strip()
+            msg = f"{year}年{month}月共使用{total_cost_np}NP"
+            if rest_np is not None:
+                msg += f"，剩余{rest_np}NP"
+            msg = (msg + "\n\n" + sio.getvalue()).strip()
 
             await MessageFactory(msg).send(reply=True)
 
 
 naga_statistic_this_month_matcher = on_command("naga本月使用情况", priority=5, block=True)
 statistic_srv.patch_matcher(naga_statistic_this_month_matcher)
 
 
 @naga_statistic_this_month_matcher.handle()
 @handle_error()
 async def naga_statistic_this_month(bot: Bot):
     cur = datetime.now(tz=TZ_TOKYO)
-    await naga_statistic(bot, cur.year, cur.month)
+    statistic = await naga.statistic(cur.year, cur.month)
+    rest_np = await naga.get_rest_np()
+    await naga_statistic(bot, cur.year, cur.month, statistic, rest_np)
 
 
 naga_statistic_prev_month_matcher = on_command("naga上月使用情况", priority=5, block=True)
 statistic_srv.patch_matcher(naga_statistic_prev_month_matcher)
 
 
 @naga_statistic_prev_month_matcher.handle()
 @handle_error()
 async def naga_statistic_prev_month(bot: Bot):
     prev_month = datetime.now(tz=TZ_TOKYO) - monthdelta(months=1)
-    await naga_statistic(bot, prev_month.year, prev_month.month)
+    statistic = await naga.statistic(prev_month.year, prev_month.month)
+    await naga_statistic(bot, prev_month.year, prev_month.month, statistic)
```

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import re
 from typing import Dict, List, Union, Sequence
 
 from httpx import AsyncClient
 from nonebot import logger
 from pydantic import BaseModel
 
 from .model import NagaReport, NagaOrder, NagaHanchanModelType, NagaTonpuuModelType, NagaGameRule
@@ -16,15 +17,15 @@
 
 class AnalyzeTenhou(BaseModel):
     status: int = 200
     msg: str = ""
 
 
 class NagaApi:
-    _BASE_URL = "https://naga.dmv.nico/naga_report/api"
+    _BASE_URL = "https://naga.dmv.nico/naga_report"
 
     _HEADER = {
         "Cache-Control": "no-cache",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.35",
     }
 
     def __init__(self, cookies: Dict[str, str]):
@@ -45,15 +46,15 @@
         )
 
     async def close(self):
         await self.client.aclose()
 
     async def order_report_list(self, year: int, month: int) -> OrderReportList:
         resp = await self.client.get(
-            "/order_report_list/",
+            "/api/order_report_list/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_report_list/"
             },
             params={"year": year, "month": month}
         )
         return OrderReportList.parse_obj(resp.json())
 
@@ -66,15 +67,15 @@
             "seat": seat,
             "reanalysis": 0,
             "player_types": model_type_to_str(model_type),
             "csrfmiddlewaretoken": self.client.cookies["csrftoken"]
         }
 
         resp = await self.client.post(
-            "/url_analyze/",
+            "/api/url_analyze/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_form/"
             },
             data=data
         )
 
         if len(resp.content) > 0:
@@ -94,13 +95,22 @@
             "seat": seat,
             "game_type": rule.value,
             "player_types": model_type_to_str(model_type),
             "csrfmiddlewaretoken": self.client.cookies["csrftoken"]
         }
 
         await self.client.post(
-            "/custom_haihu_analyze/",
+            "/api/custom_haihu_analyze/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_form/"
             },
             data=res_data
         )
+
+    async def get_rest_np(self) -> int:
+        resp = await self.client.get(
+            "/order_form/"
+        )
+        mat = re.search(r"const base_left_point = (\d+)", resp.text)
+        if mat is None:
+            raise RuntimeError("cannot get base_left_point")
+        return int(mat.group(1))
```

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from nonebot_plugin_nagabus.utils.tz import TZ_TOKYO
 
 
 class FakeNagaApi:
     def __init__(self):
         self.report = []
         self.order = []
+        self.rest_np = 1500
 
     async def close(self):
         ...
 
     async def order_report_list(self, year: int, month: int) -> OrderReportList:
         return OrderReportList(report=self.report, order=self.order)
 
@@ -46,14 +47,16 @@
         time = datetime.now(tz=TZ_TOKYO).replace(tzinfo=None).isoformat(timespec='seconds')
         feat = ''.join(str(random.randint(1, 9)) for _ in range(16))
         haihu_id = f"custom_haihu_{time}_{feat}"
         order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok,
                           model=NagaModel(2, 2, 0, model_type_to_str(model_type)), rule=rule)
         create_task(self._produce_order(order))
 
+        self.rest_np -= 10
+
         report_id = str(uuid4())
         report = NagaReport(haihu_id=haihu_id, players=[NagaReportPlayer("AI", 0)] * 4, report_id=report_id, seat=0,
                             model=NagaModel(2, 2, 0, model_type_to_str(model_type)), rule=rule)
         create_task(self._produce_report(report))
 
     async def analyze_tenhou(self, haihu_id: str, seat: int,
                              rule: NagaGameRule,
@@ -64,13 +67,21 @@
                 return AnalyzeTenhou(status=400, msg="すでに解析済みの牌譜です")
 
         order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok,
                           model=NagaModel(2, 2, 0, model_type_to_str(model_type)),
                           rule=NagaGameRule.hanchan)
         create_task(self._produce_order(order))
 
+        if rule == NagaGameRule.hanchan:
+            self.rest_np -= 50
+        else:
+            self.rest_np -= 30
+
         report_id = str(uuid4())
         report = NagaReport(haihu_id=haihu_id, players=[NagaReportPlayer("AI", 0)] * 4, report_id=report_id, seat=seat,
                             model=NagaModel(2, 2, 0, model_type_to_str(model_type)), rule=NagaGameRule.hanchan)
         create_task(self._produce_report(report))
 
         return AnalyzeTenhou(status=200, msg="")
+
+    async def get_resp_np(self) -> int:
+        return self.rest_np
```

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,7 +461,10 @@
             if order.customer_id not in statistic:
                 statistic[order.customer_id] = 0
             statistic[order.customer_id] += order.cost_np
 
         statistic = [NagaServiceUserStatistic(x[0], x[1]) for x in statistic.items()]
         statistic.sort(key=lambda x: x.cost_np, reverse=True)
         return statistic
+
+    async def get_rest_np(self) -> int:
+        return await self.api.get_rest_np()
```

### Comparing `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/pyproject.toml` & `nonebot_plugin_nagabus-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.2.3/README.md` & `nonebot_plugin_nagabus-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.3/PKG-INFO` & `nonebot_plugin_nagabus-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

