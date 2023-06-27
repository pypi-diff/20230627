# Comparing `tmp/nonebot_plugin_boardgame-0.2.1.tar.gz` & `tmp/nonebot_plugin_boardgame-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_boardgame-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_boardgame-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_boardgame-0.2.1.tar` & `nonebot_plugin_boardgame-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1675 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/README.md
--rw-r--r--   0        0        0    12989 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/__init__.py
--rw-r--r--   0        0        0    10569 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/game.py
--rw-r--r--   0        0        0     2005 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/go.py
--rw-r--r--   0        0        0     2028 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/gomoku.py
--rw-r--r--   0        0        0     1451 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/migrations/b737d3c58568_init_db.py
--rw-r--r--   0        0        0     1295 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/model.py
--rw-r--r--   0        0        0     2414 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/othello.py
--rw-r--r--   0        0        0     3635 2023-03-10 12:07:11.412455 nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/svg.py
--rw-r--r--   0        0        0      774 2023-03-10 12:07:11.416455 nonebot_plugin_boardgame-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 nonebot_plugin_boardgame-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1675 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/README.md
+-rw-r--r--   0        0        0    12140 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/__init__.py
+-rw-r--r--   0        0        0    10596 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/game.py
+-rw-r--r--   0        0        0     2005 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/go.py
+-rw-r--r--   0        0        0     2028 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/gomoku.py
+-rw-r--r--   0        0        0     1451 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/migrations/b737d3c58568_init_db.py
+-rw-r--r--   0        0        0     1295 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/model.py
+-rw-r--r--   0        0        0     2414 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/othello.py
+-rw-r--r--   0        0        0     3635 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/svg.py
+-rw-r--r--   0        0        0      866 2023-06-27 11:41:33.829751 nonebot_plugin_boardgame-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 nonebot_plugin_boardgame-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_boardgame-0.2.1/README.md` & `nonebot_plugin_boardgame-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/__init__.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 import asyncio
 import shlex
 from asyncio import TimerHandle
 from dataclasses import dataclass
-from typing import Dict, List, NoReturn, Optional, Union
+from typing import Dict, List, NoReturn, Optional
 
 from nonebot import on_command, on_shell_command, require
-from nonebot.adapters.onebot.v11 import Bot as V11Bot
-from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
-from nonebot.adapters.onebot.v11 import Message as V11Msg
-from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
-from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
-from nonebot.adapters.onebot.v11 import PrivateMessageEvent as V11PMEvent
-from nonebot.adapters.onebot.v12 import Bot as V12Bot
-from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12CMEvent
-from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12GMEvent
-from nonebot.adapters.onebot.v12 import Message as V12Msg
-from nonebot.adapters.onebot.v12 import MessageEvent as V12MEvent
-from nonebot.adapters.onebot.v12 import MessageSegment as V12MsgSeg
-from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12PMEvent
+from nonebot.adapters import Bot, Event, Message
 from nonebot.exception import ParserExit
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, CommandStart, EventToMe, ShellCommandArgv
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import ArgumentParser, Rule
 
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
+require("nonebot_plugin_userinfo")
 require("nonebot_plugin_datastore")
 require("nonebot_plugin_htmlrender")
 
+from nonebot_plugin_saa import Image, MessageFactory
+from nonebot_plugin_saa import __plugin_meta__ as saa_plugin_meta
+from nonebot_plugin_session import SessionIdType, SessionLevel
+from nonebot_plugin_session import __plugin_meta__ as session_plugin_meta
+from nonebot_plugin_session import extract_session
+from nonebot_plugin_userinfo import __plugin_meta__ as userinfo_plugin_meta
+from nonebot_plugin_userinfo import get_user_info
+
+assert saa_plugin_meta.supported_adapters
+assert session_plugin_meta.supported_adapters
+assert userinfo_plugin_meta.supported_adapters
+supported_adapters = (
+    saa_plugin_meta.supported_adapters
+    & session_plugin_meta.supported_adapters
+    & userinfo_plugin_meta.supported_adapters
+)
+
 from .game import Game, MoveResult, Player, Pos
 from .go import Go
 from .gomoku import Gomoku
 from .othello import Othello
 
 __plugin_meta__ = PluginMetadata(
     name="棋类游戏",
     description="五子棋、黑白棋、围棋",
     usage=(
         "@我 + “五子棋”、“黑白棋”、“围棋”开始一局游戏;\n"
         "再发送“落子 字母+数字”下棋，如“落子 A1”;\n"
         "发送“结束下棋”结束当前棋局；发送“显示棋盘”显示当前棋局"
     ),
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-boardgame",
+    supported_adapters=supported_adapters,
     extra={
         "unique_name": "boardgame",
         "example": "@小Q 五子棋\n落子 G8\n结束下棋",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.1",
+        "version": "0.3.0",
     },
 )
 
 
 parser = ArgumentParser("boardgame", description="棋类游戏")
 parser.add_argument("-r", "--rule", help="棋局规则")
 group = parser.add_mutually_exclusive_group()
@@ -62,69 +73,58 @@
 
 
 boardgame = on_shell_command("boardgame", parser=parser, block=True, priority=13)
 
 
 @boardgame.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str] = ShellCommandArgv(),
 ):
     await handle_boardgame(bot, matcher, event, argv)
 
 
 def shortcut(cmd: str, argv: List[str] = [], **kwargs):
     command = on_command(cmd, **kwargs, block=True, priority=13)
 
     @command.handle()
     async def _(
-        bot: Union[V11Bot, V12Bot],
+        bot: Bot,
         matcher: Matcher,
-        event: Union[V11MEvent, V12MEvent],
-        msg: Union[V11Msg, V12Msg] = CommandArg(),
+        event: Event,
+        msg: Message = CommandArg(),
     ):
         try:
             args = shlex.split(msg.extract_plain_text().strip())
         except:
             args = []
         await handle_boardgame(bot, matcher, event, argv + args)
 
 
-def get_cid(bot: Union[V11Bot, V12Bot], event: Union[V11MEvent, V12MEvent]):
-    if isinstance(event, V11MEvent):
-        cid = f"{bot.self_id}_{event.sub_type}_"
-    else:
-        cid = f"{bot.self_id}_{event.detail_type}_"
-
-    if isinstance(event, V11GMEvent) or isinstance(event, V12GMEvent):
-        cid += str(event.group_id)
-    elif isinstance(event, V12CMEvent):
-        cid += f"{event.guild_id}_{event.channel_id}"
-    else:
-        cid += str(event.user_id)
-
-    return cid
-
-
-def game_running(
-    bot: Union[V11Bot, V12Bot], event: Union[V11MEvent, V12MEvent]
-) -> bool:
+def get_cid(bot: Bot, event: Event):
+    return extract_session(bot, event).get_id(SessionIdType.GROUP)
+
+
+def game_running(bot: Bot, event: Event) -> bool:
     cid = get_cid(bot, event)
     return bool(games.get(cid, None))
 
 
 # 命令前缀为空则需要to_me，否则不需要
 def smart_to_me(command_start: str = CommandStart(), to_me: bool = EventToMe()) -> bool:
     return bool(command_start) or to_me
 
 
-def not_private(event: Union[V11MEvent, V12MEvent]) -> bool:
-    return not (isinstance(event, V11PMEvent) or isinstance(event, V12PMEvent))
+def not_private(bot: Bot, event: Event) -> bool:
+    return extract_session(bot, event).level not in (
+        SessionLevel.LEVEL0,
+        SessionLevel.LEVEL1,
+    )
 
 
 shortcut("五子棋", ["--rule", "gomoku"], rule=Rule(smart_to_me) & not_private)
 shortcut(
     "黑白棋", ["--rule", "othello"], aliases={"奥赛罗"}, rule=Rule(smart_to_me) & not_private
 )
 shortcut("围棋", ["--rule", "go"], rule=Rule(smart_to_me) & not_private)
@@ -169,51 +169,41 @@
     timer = loop.call_later(
         timeout, lambda: asyncio.ensure_future(stop_game(matcher, cid))
     )
     timers[cid] = timer
 
 
 async def handle_boardgame(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str],
 ):
-    async def new_player(event: Union[V11MEvent, V12MEvent]) -> Player:
+    async def new_player(event: Event) -> Player:
         user_id = event.get_user_id()
         user_name = ""
-        if isinstance(event, V11MEvent):
-            user_name = event.sender.card or event.sender.nickname or ""
-        else:
-            assert isinstance(bot, V12Bot)
-            resp = await bot.get_user_info(user_id=user_id)
-            user_name = resp["user_displayname"] or resp["user_name"]
+        if user_info := await get_user_info(bot, event, user_id=user_id):
+            user_name = user_info.user_name
         return Player(user_id, user_name)
 
     async def send(
         message: Optional[str] = None, image: Optional[bytes] = None
     ) -> NoReturn:
         if not (message or image):
             await matcher.finish()
 
-        if isinstance(bot, V11Bot):
-            msg = V11Msg()
-            if message:
-                msg.append(message)
-            if image:
-                msg.append(V11MsgSeg.image(image))
-        else:
-            msg = V12Msg()
-            if message:
-                msg.append(message)
+        msg_builder = MessageFactory([])
+        if message:
             if image:
-                resp = await bot.upload_file(type="data", name="boardgame", data=image)
-                file_id = resp["file_id"]
-                msg.append(V12MsgSeg.image(file_id))
-        await matcher.finish(msg)
+                message += "\n"
+            msg_builder.append(message)
+        if image:
+            msg_builder.append(Image(image))
+        await msg_builder.send()
+        await matcher.finish()
 
     try:
         args = parser.parse_args(argv)
     except ParserExit as e:
         if e.status == 0:
             await send(__plugin_meta__.usage)
         await send()
```

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/game.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,17 @@
             record.player_black_id, record.player_black_name
         )
         game.player_white = load_player(
             record.player_white_id, record.player_white_name
         )
         game.start_time = record.start_time
         game.update_time = record.update_time
-        positions = [Pos.from_str(pos) for pos in record.positions.split(" ") if pos]
+        positions = [
+            Pos.from_str(pos) for pos in str(record.positions).split(" ") if pos
+        ]
         for pos in positions:
             game.update(pos)
         return game
 
     def draw_svg(self):
         size = self.size
         placement = self.placement
```

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/go.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/go.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/gomoku.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/gomoku.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/migrations/b737d3c58568_init_db.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/migrations/b737d3c58568_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/model.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/othello.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/othello.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/nonebot_plugin_boardgame/svg.py` & `nonebot_plugin_boardgame-0.3.0/nonebot_plugin_boardgame/svg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_boardgame-0.2.1/PKG-INFO` & `nonebot_plugin_boardgame-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-boardgame
-Version: 0.2.1
+Version: 0.3.0
 Summary: 适用于 Nonebot2 的棋类游戏插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-boardgame
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot-plugin-datastore (>=0.6.0a1,<0.7.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.0.4)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-plugin-datastore (>=1.0.0,<2.0.0)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.5,<0.1.0)
+Requires-Dist: nonebot-plugin-userinfo (>=0.0.1,<0.1.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-boardgame
 Description-Content-Type: text/markdown
 
 ## nonebot-plugin-boardgame
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的棋类游戏插件。
```

