# Comparing `tmp/nonebot_plugin_chess-0.3.1.tar.gz` & `tmp/nonebot_plugin_chess-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chess-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_chess-0.4.0.tar", max compression
```

## Comparing `nonebot_plugin_chess-0.3.1.tar` & `nonebot_plugin_chess-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/LICENSE
--rw-r--r--   0        0        0     1968 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/README.md
--rw-r--r--   0        0        0    15792 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/__init__.py
--rw-r--r--   0        0        0      170 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/config.py
--rw-r--r--   0        0        0     6637 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/game.py
--rw-r--r--   0        0        0     1728 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py
--rw-r--r--   0        0        0     1705 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/model.py
--rw-r--r--   0        0        0      762 2023-03-10 11:59:26.938872 nonebot_plugin_chess-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 nonebot_plugin_chess-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1968 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/README.md
+-rw-r--r--   0        0        0    14756 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/config.py
+-rw-r--r--   0        0        0     6637 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/game.py
+-rw-r--r--   0        0        0     1728 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py
+-rw-r--r--   0        0        0     1705 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/model.py
+-rw-r--r--   0        0        0      854 2023-06-27 11:15:28.546989 nonebot_plugin_chess-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 nonebot_plugin_chess-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_chess-0.3.1/LICENSE` & `nonebot_plugin_chess-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.3.1/README.md` & `nonebot_plugin_chess-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/__init__.py` & `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,62 +4,72 @@
 from asyncio import TimerHandle
 from dataclasses import dataclass
 from typing import Dict, Iterable, List, NoReturn, Union
 
 import chess
 from chess import Termination
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
 
-require("nonebot_plugin_htmlrender")
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
 from .config import Config
 from .game import AiPlayer, Game, Player
 
 __plugin_meta__ = PluginMetadata(
     name="国际象棋",
     description="国际象棋，支持人机和对战",
     usage=(
         "@我 + “国际象棋人机”或“国际象棋对战”开始一局游戏；\n"
         "可使用“lv1~8”指定AI等级，如“国际象棋人机lv5”，默认为“lv4”；\n"
         "发送 起始坐标格式，如“e2e4”下棋；\n"
         "在坐标后加棋子字母表示升变，如“e7e8q”表示升变为后；\n"
         "发送“结束下棋”结束当前棋局；发送“显示棋盘”显示当前棋局"
     ),
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-chess",
     config=Config,
+    supported_adapters=supported_adapters,
     extra={
         "unique_name": "chess",
         "example": "@小Q 国际象棋人机lv5\ne2e4\n结束下棋",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.3.1",
+        "version": "0.4.0",
     },
 )
 
 
 parser = ArgumentParser("chess", description="国际象棋")
 group = parser.add_mutually_exclusive_group()
 group.add_argument("-e", "--stop", "--end", action="store_true", help="停止下棋")
@@ -89,69 +99,58 @@
 
 
 chess_matcher = on_shell_command("chess", parser=parser, block=True, priority=13)
 
 
 @chess_matcher.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str] = ShellCommandArgv(),
 ):
     await handle_chess(bot, matcher, event, argv)
 
 
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
         await handle_chess(bot, matcher, event, argv + args)
 
 
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
 
 
 shortcut(
     "国际象棋对战", ["--battle"], aliases={"国际象棋双人"}, rule=Rule(smart_to_me) & not_private
 )
 shortcut("国际象棋人机", aliases={"国际象棋单人"}, rule=smart_to_me)
 for i in range(1, 9):
@@ -180,17 +179,17 @@
 
 
 move_matcher = on_message(Rule(game_running) & get_move_input, block=True, priority=14)
 
 
 @move_matcher.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     state: T_State,
 ):
     move: str = state["move"]
     await handle_chess(bot, matcher, event, [move])
 
 
 async def stop_game(cid: str):
@@ -214,53 +213,40 @@
     timer = loop.call_later(
         timeout, lambda: asyncio.ensure_future(stop_game_timeout(matcher, cid))
     )
     timers[cid] = timer
 
 
 async def handle_chess(
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
 
     async def send(msgs: Union[str, Iterable[Union[str, bytes]]] = "") -> NoReturn:
         if not msgs:
             await matcher.finish()
         if isinstance(msgs, str):
             await matcher.finish(msgs)
 
-        if isinstance(bot, V11Bot):
-            message = V11Msg()
-            for msg in msgs:
-                if isinstance(msg, bytes):
-                    message.append(V11MsgSeg.image(msg))
-                else:
-                    message.append(msg)
-        else:
-            message = V12Msg()
-            for msg in msgs:
-                if isinstance(msg, bytes):
-                    resp = await bot.upload_file(type="data", name="chess", data=msg)
-                    file_id = resp["file_id"]
-                    message.append(V12MsgSeg.image(file_id))
-                else:
-                    message.append(msg)
-        await matcher.finish(message)
+        msg_builder = MessageFactory([])
+        for msg in msgs:
+            if isinstance(msg, bytes):
+                msg_builder.append(Image(msg))
+            else:
+                msg_builder.append(msg)
+        await msg_builder.send()
+        await matcher.finish()
 
     try:
         args = parser.parse_args(argv)
     except ParserExit as e:
         if e.status == 0:
             await matcher.finish(__plugin_meta__.usage)
         await matcher.finish()
@@ -288,15 +274,15 @@
             games[cid] = game
             await send(
                 (
                     (
                         f"游戏发起时间：{game.start_time.strftime('%Y-%m-%d %H:%M:%S')}\n"
                         f"白方：{game.player_white}\n"
                         f"黑方：{game.player_black}\n"
-                        f"下一手轮到：{game.player_next}"
+                        f"下一手轮到：{game.player_next}\n"
                     ),
                     await game.draw(),
                 )
             )
 
         game = Game()
         player = await new_player(event)
@@ -323,15 +309,15 @@
                     game.player_black = ai_player
             except:
                 await send("国际象棋引擎加载失败，请检查设置")
 
         games[cid] = game
         set_timeout(matcher, cid)
         await game.save_record(cid)
-        await send((msg, await game.draw()))
+        await send((msg + "\n", await game.draw()))
 
     game = games[cid]
     set_timeout(matcher, cid)
     player = await new_player(event)
 
     if options.stop:
         if (not game.player_white or game.player_white != player) and (
@@ -361,15 +347,15 @@
             game.board.pop()
         else:
             if len(game.board.move_stack) <= 1 and game.player_last != player:
                 await send("上一手棋不是你所下")
             game.board.pop()
             game.board.pop()
         await game.save_record(cid)
-        await send((f"{player} 进行了悔棋", await game.draw()))
+        await send((f"{player} 进行了悔棋\n", await game.draw()))
 
     if (game.player_next and game.player_next != player) or (
         game.player_last and game.player_last == player
     ):
         await send("当前不是你的回合")
 
     move = options.move
@@ -409,15 +395,15 @@
         elif result in [Termination.INSUFFICIENT_MATERIAL, Termination.STALEMATE]:
             msg += f"，本局游戏平局"
         else:
             msg += f"，游戏结束"
     else:
         if game.player_next and game.is_battle:
             msg += f"，下一手轮到 {game.player_next}"
-    msgs.append(msg)
+    msgs.append(msg + "\n")
     msgs.append(await game.draw())
 
     if not game.is_battle:
         if not game.board.is_game_over():
             ai_player = game.player_next
             assert isinstance(ai_player, AiPlayer)
             try:
@@ -425,26 +411,26 @@
                 if not move:
                     await send("国际象棋引擎出错，请结束游戏或稍后再试")
                 game.board.push_uci(move.uci())
                 result = game.board.outcome()
             except:
                 await send("国际象棋引擎出错，请结束游戏或稍后再试")
 
-            msg = f"{ai_player} 下出 {move}"
+            msg = f"\n{ai_player} 下出 {move}"
             if game.board.is_game_over():
                 await stop_game(cid)
                 if result == Termination.CHECKMATE:
                     winner = result.winner
                     assert winner is not None
                     msg += "，恭喜你赢了！" if game.board.turn == (not winner) else "，很遗憾你输了！"
                 elif result in [
                     Termination.INSUFFICIENT_MATERIAL,
                     Termination.STALEMATE,
                 ]:
                     msg += f"，本局游戏平局"
                 else:
                     msg += f"，游戏结束"
-            msgs.append(msg)
+            msgs.append(msg + "\n")
             msgs.append((await game.draw()))
 
     await game.save_record(cid)
     await send(msgs)
```

### Comparing `nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/game.py` & `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py` & `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.3.1/nonebot_plugin_chess/model.py` & `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.3.1/pyproject.toml` & `nonebot_plugin_chess-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "nonebot_plugin_chess"
-version = "0.3.1"
+version = "0.4.0"
 description = "Nonebot2 国际象棋插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-chess"
 repository = "https://github.com/noneplugin/nonebot-plugin-chess"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+nonebot-plugin-session = ">=0.0.5,<0.1.0"
+nonebot-plugin-userinfo = ">=0.0.1,<0.1.0"
+nonebot-plugin-datastore = "^1.0.0"
+nonebot-plugin-htmlrender = "^0.2.0"
 chess = "^1.9.0"
-nonebot-plugin-htmlrender = ">=0.0.4"
-nonebot-plugin-datastore = "^0.6.0a1"
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.0.0"
 black = "^22.1.0"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_chess"]
```

### Comparing `nonebot_plugin_chess-0.3.1/PKG-INFO` & `nonebot_plugin_chess-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chess
-Version: 0.3.1
+Version: 0.4.0
 Summary: Nonebot2 国际象棋插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-chess
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
 Requires-Dist: chess (>=1.9.0,<2.0.0)
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
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-chess
 Description-Content-Type: text/markdown
 
 ## nonebot-plugin-chess
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的国际象棋插件。
```

