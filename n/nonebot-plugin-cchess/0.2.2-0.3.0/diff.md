# Comparing `tmp/nonebot_plugin_cchess-0.2.2.tar.gz` & `tmp/nonebot_plugin_cchess-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cchess-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_cchess-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_cchess-0.2.2.tar` & `nonebot_plugin_cchess-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/LICENSE
--rw-r--r--   0        0        0     2252 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/README.md
--rw-r--r--   0        0        0    15886 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/__init__.py
--rw-r--r--   0        0        0    15389 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/board.py
--rw-r--r--   0        0        0      178 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/config.py
--rw-r--r--   0        0        0     1522 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/drawer.py
--rw-r--r--   0        0        0     2453 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/engine.py
--rw-r--r--   0        0        0     5322 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/game.py
--rw-r--r--   0        0        0     1722 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/migrations/2c0cbe227dd9_init_db.py
--rw-r--r--   0        0        0     1755 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/model.py
--rw-r--r--   0        0        0    11675 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/move.py
--rw-r--r--   0        0        0     1392 2023-03-10 11:41:45.206559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/piece.py
--rw-r--r--   0        0        0    71284 2023-03-10 11:41:45.210559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/a_black.png
--rw-r--r--   0        0        0    79093 2023-03-10 11:41:45.210559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/a_red.png
--rw-r--r--   0        0        0    80466 2023-03-10 11:41:45.210559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/b_black.png
--rw-r--r--   0        0        0    82540 2023-03-10 11:41:45.210559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/b_red.png
--rw-r--r--   0        0        0   212046 2023-03-10 11:41:45.210559 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/board_black.png
--rw-r--r--   0        0        0   212711 2023-03-10 11:41:45.214558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/board_red.png
--rw-r--r--   0        0        0    78800 2023-03-10 11:41:45.214558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/c_black.png
--rw-r--r--   0        0        0    83546 2023-03-10 11:41:45.214558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/c_red.png
--rw-r--r--   0        0        0    78458 2023-03-10 11:41:45.214558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/k_black.png
--rw-r--r--   0        0        0    83683 2023-03-10 11:41:45.214558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/k_red.png
--rw-r--r--   0        0        0     4788 2023-03-10 11:41:45.214558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/mark.png
--rw-r--r--   0        0        0    75484 2023-03-10 11:41:45.218558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/n_black.png
--rw-r--r--   0        0        0    84914 2023-03-10 11:41:45.218558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/n_red.png
--rw-r--r--   0        0        0    73821 2023-03-10 11:41:45.218558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/p_black.png
--rw-r--r--   0        0        0    79975 2023-03-10 11:41:45.218558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/p_red.png
--rw-r--r--   0        0        0    74655 2023-03-10 11:41:45.218558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/r_black.png
--rw-r--r--   0        0        0    83880 2023-03-10 11:41:45.218558 nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/r_red.png
--rw-r--r--   0        0        0      723 2023-03-10 11:41:45.222558 nonebot_plugin_cchess-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 nonebot_plugin_cchess-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2252 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/README.md
+-rw-r--r--   0        0        0    14787 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/__init__.py
+-rw-r--r--   0        0        0    15389 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/board.py
+-rw-r--r--   0        0        0      178 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/config.py
+-rw-r--r--   0        0        0     1521 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/drawer.py
+-rw-r--r--   0        0        0     2453 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/engine.py
+-rw-r--r--   0        0        0     5322 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/game.py
+-rw-r--r--   0        0        0     1722 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/migrations/2c0cbe227dd9_init_db.py
+-rw-r--r--   0        0        0     1755 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/model.py
+-rw-r--r--   0        0        0    11675 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/move.py
+-rw-r--r--   0        0        0     1392 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/piece.py
+-rw-r--r--   0        0        0    71284 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/a_black.png
+-rw-r--r--   0        0        0    79093 2023-06-27 07:39:16.563475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/a_red.png
+-rw-r--r--   0        0        0    80466 2023-06-27 07:39:16.567475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/b_black.png
+-rw-r--r--   0        0        0    82540 2023-06-27 07:39:16.567475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/b_red.png
+-rw-r--r--   0        0        0   212046 2023-06-27 07:39:16.567475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/board_black.png
+-rw-r--r--   0        0        0   212711 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/board_red.png
+-rw-r--r--   0        0        0    78800 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/c_black.png
+-rw-r--r--   0        0        0    83546 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/c_red.png
+-rw-r--r--   0        0        0    78458 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/k_black.png
+-rw-r--r--   0        0        0    83683 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/k_red.png
+-rw-r--r--   0        0        0     4788 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/mark.png
+-rw-r--r--   0        0        0    75484 2023-06-27 07:39:16.571475 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/n_black.png
+-rw-r--r--   0        0        0    84914 2023-06-27 07:39:16.575476 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/n_red.png
+-rw-r--r--   0        0        0    73821 2023-06-27 07:39:16.575476 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/p_black.png
+-rw-r--r--   0        0        0    79975 2023-06-27 07:39:16.575476 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/p_red.png
+-rw-r--r--   0        0        0    74655 2023-06-27 07:39:16.575476 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/r_black.png
+-rw-r--r--   0        0        0    83880 2023-06-27 07:39:16.575476 nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/r_red.png
+-rw-r--r--   0        0        0      816 2023-06-27 07:39:16.575476 nonebot_plugin_cchess-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 nonebot_plugin_cchess-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_cchess-0.2.2/LICENSE` & `nonebot_plugin_cchess-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/README.md` & `nonebot_plugin_cchess-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/__init__.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,42 +3,50 @@
 import shlex
 from asyncio import TimerHandle
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Dict, Iterable, List, NoReturn, Union
 
 from nonebot import on_command, on_message, on_shell_command, require
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
 from nonebot.params import (
     CommandArg,
     CommandStart,
     EventPlainText,
     EventToMe,
     ShellCommandArgv,
 )
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import ArgumentParser, Rule
 from nonebot.typing import T_State
 
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
+require("nonebot_plugin_userinfo")
 require("nonebot_plugin_datastore")
 
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
 from .board import MoveResult
 from .config import Config
 from .engine import EngineError
 from .game import AiPlayer, Game, Player
 from .move import Move
 
 __plugin_meta__ = PluginMetadata(
@@ -46,15 +54,18 @@
     description="象棋，支持人机和对战",
     usage=(
         "@我 + “象棋人机”或“象棋对战”开始一局游戏；\n"
         "可使用“lv1~8”指定AI等级，如“象棋人机lv5”，默认为“lv4”；\n"
         "发送 中文纵线格式如“炮二平五” 或 起始坐标格式如“h2e2”下棋；\n"
         "发送“结束下棋”结束当前棋局；发送“显示棋盘”显示当前棋局"
     ),
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-cchess",
     config=Config,
+    supported_adapters=supported_adapters,
     extra={
         "unique_name": "cchess",
         "example": "@小Q 象棋人机lv5\n炮二平五\n结束下棋",
         "author": "meetwq <meetwq@gmail.com>",
         "version": "0.2.2",
     },
 )
@@ -89,69 +100,53 @@
 
 
 cchess = on_shell_command("cchess", parser=parser, block=True, priority=13)
 
 
 @cchess.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str] = ShellCommandArgv(),
 ):
     await handle_cchess(bot, matcher, event, argv)
 
 
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
+def get_cid(bot: Bot, event: Event):
+    return extract_session(bot, event).get_id(SessionIdType.GROUP)
 
 
 def shortcut(cmd: str, argv: List[str] = [], **kwargs):
     command = on_command(cmd, **kwargs, block=True, priority=13)
 
     @command.handle()
-    async def _(
-        bot: Union[V11Bot, V12Bot],
-        matcher: Matcher,
-        event: Union[V11MEvent, V12MEvent],
-        msg: Union[V11Msg, V12Msg] = CommandArg(),
-    ):
+    async def _(bot: Bot, matcher: Matcher, event: Event, msg: Message = CommandArg()):
         try:
             args = shlex.split(msg.extract_plain_text().strip())
         except:
             args = []
         await handle_cchess(bot, matcher, event, argv + args)
 
 
-def game_running(
-    bot: Union[V11Bot, V12Bot], event: Union[V11MEvent, V12MEvent]
-) -> bool:
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
 
 
 shortcut("象棋对战", ["--battle"], aliases={"象棋双人"}, rule=Rule(smart_to_me) & not_private)
 shortcut("象棋人机", aliases={"象棋单人"}, rule=smart_to_me)
 for i in range(1, 9):
     shortcut(
         f"象棋人机lv{i}",
@@ -178,17 +173,17 @@
 
 
 pos_matcher = on_message(Rule(game_running) & get_move_input, block=True, priority=14)
 
 
 @pos_matcher.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     state: T_State,
 ):
     move: str = state["move"]
     await handle_cchess(bot, matcher, event, [move])
 
 
 def stop_game(cid: str):
@@ -212,55 +207,40 @@
     timer = loop.call_later(
         timeout, lambda: asyncio.ensure_future(stop_game_timeout(matcher, cid))
     )
     timers[cid] = timer
 
 
 async def handle_cchess(
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
 
     async def send(msgs: Union[str, Iterable[Union[str, BytesIO]]] = "") -> NoReturn:
         if not msgs:
             await matcher.finish()
         if isinstance(msgs, str):
             await matcher.finish(msgs)
 
-        if isinstance(bot, V11Bot):
-            message = V11Msg()
-            for msg in msgs:
-                if isinstance(msg, BytesIO):
-                    message.append(V11MsgSeg.image(msg))
-                else:
-                    message.append(msg)
-        else:
-            message = V12Msg()
-            for msg in msgs:
-                if isinstance(msg, BytesIO):
-                    resp = await bot.upload_file(
-                        type="data", name="cchess", data=msg.getvalue()
-                    )
-                    file_id = resp["file_id"]
-                    message.append(V12MsgSeg.image(file_id))
-                else:
-                    message.append(msg)
-        await matcher.finish(message)
+        msg_builder = MessageFactory([])
+        for msg in msgs:
+            if isinstance(msg, BytesIO):
+                msg_builder.append(Image(msg))
+            else:
+                msg_builder.append(msg)
+        await msg_builder.send()
+        await matcher.finish()
 
     try:
         args = parser.parse_args(argv)
     except ParserExit as e:
         if e.status == 0:
             await send(__plugin_meta__.usage)
         await send()
@@ -324,15 +304,15 @@
                     game.player_black = ai_player
             except EngineError:
                 await send("象棋引擎加载失败，请检查设置")
 
         games[cid] = game
         set_timeout(matcher, cid)
         await game.save_record(cid)
-        await send((msg, game.draw()))
+        await send((msg + "\n", game.draw()))
 
     game = games[cid]
     set_timeout(matcher, cid)
     player = await new_player(event)
 
     if options.stop:
         if (not game.player_red or game.player_red != player) and (
@@ -362,15 +342,15 @@
             game.pop()
         else:
             if len(game.history) <= 2 and game.player_last != player:
                 await send("上一手棋不是你所下")
             game.pop()
             game.pop()
         await game.save_record(cid)
-        await send((f"{player} 进行了悔棋", game.draw()))
+        await send((f"{player} 进行了悔棋\n", game.draw()))
 
     if (game.player_next and game.player_next != player) or (
         game.player_last and game.player_last == player
     ):
         await send("当前不是你的回合")
 
     move = options.move
@@ -422,39 +402,39 @@
     elif result == MoveResult.DRAW:
         stop_game(cid)
         msg += f"，本局游戏平局"
     else:
         if game.player_next and game.is_battle:
             msg += f"，下一手轮到 {game.player_next}"
 
-    msgs.append(msg)
+    msgs.append(msg + "\n")
 
     if game.is_battle:
         msgs.append(game.draw())
     else:
         msgs.append(game.draw(False))
         if not result:
             ai_player = game.player_next
             assert isinstance(ai_player, AiPlayer)
             move = await ai_player.get_move(game.position())
             move_chi = move.chinese(game)
             result = game.push(move)
 
-            msg = f"{ai_player} 下出 {move_chi}"
+            msg = f"\n{ai_player} 下出 {move_chi}"
             if result == MoveResult.ILLEAGAL:
                 game.pop()
                 await send("象棋引擎出错，请结束游戏或稍后再试")
             elif result:
                 stop_game(cid)
                 if result == MoveResult.CHECKED:
                     msg += "，恭喜你赢了！"
                 elif result == MoveResult.RED_WIN:
                     msg += "，恭喜你赢了！" if player == game.player_red else "，很遗憾你输了！"
                 elif result == MoveResult.BLACK_WIN:
                     msg += "，恭喜你赢了！" if player == game.player_black else "，很遗憾你输了！"
                 elif result == MoveResult.DRAW:
                     msg += f"，本局游戏平局"
-            msgs.append(msg)
+            msgs.append(msg + "\n")
             msgs.append(game.draw())
 
     await game.save_record(cid)
     await send(msgs)
```

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/board.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/board.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/drawer.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     to_pos = last_move.to_pos
     draw_mark = True
     if from_pos == to_pos:
         draw_mark = False
 
     for i, line in enumerate(pieces):
         for j, piece in enumerate(line):
-
             if side:
                 x = 200 + 300 * j
                 y = 3150 - 300 * i
             else:
                 x = 2600 - 300 * j
                 y = 450 + 300 * i
```

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/engine.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/engine.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/game.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/migrations/2c0cbe227dd9_init_db.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/migrations/2c0cbe227dd9_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/model.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/move.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/move.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/piece.py` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/piece.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/a_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/a_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/a_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/a_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/b_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/b_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/b_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/b_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/board_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/board_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/board_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/board_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/c_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/c_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/c_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/c_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/k_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/k_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/k_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/k_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/mark.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/mark.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/n_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/n_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/n_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/n_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/p_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/p_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/p_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/p_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/r_black.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/r_black.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/nonebot_plugin_cchess/resources/images/r_red.png` & `nonebot_plugin_cchess-0.3.0/nonebot_plugin_cchess/resources/images/r_red.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cchess-0.2.2/pyproject.toml` & `nonebot_plugin_cchess-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "nonebot_plugin_cchess"
-version = "0.2.2"
+version = "0.3.0"
 description = "Nonebot2 象棋插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-cchess"
 repository = "https://github.com/noneplugin/nonebot-plugin-cchess"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+nonebot-plugin-session = ">=0.0.5,<0.1.0"
+nonebot-plugin-userinfo = ">=0.0.1,<0.1.0"
+nonebot-plugin-datastore = "^1.0.0"
 Pillow = "^9.0.0"
-nonebot-plugin-datastore = "^0.6.0a1"
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.0.0"
 black = "^22.1.0"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_cchess"]
```

### Comparing `nonebot_plugin_cchess-0.2.2/PKG-INFO` & `nonebot_plugin_cchess-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cchess
-Version: 0.2.2
+Version: 0.3.0
 Summary: Nonebot2 象棋插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-cchess
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
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot-plugin-datastore (>=0.6.0a1,<0.7.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-plugin-datastore (>=1.0.0,<2.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.5,<0.1.0)
+Requires-Dist: nonebot-plugin-userinfo (>=0.0.1,<0.1.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-cchess
 Description-Content-Type: text/markdown
 
 ## nonebot-plugin-cchess
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的象棋插件。
```

