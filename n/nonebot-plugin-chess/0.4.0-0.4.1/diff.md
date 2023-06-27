# Comparing `tmp/nonebot_plugin_chess-0.4.0.tar.gz` & `tmp/nonebot_plugin_chess-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chess-0.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_chess-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_chess-0.4.0.tar` & `nonebot_plugin_chess-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/LICENSE
--rw-r--r--   0        0        0     1968 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/README.md
--rw-r--r--   0        0        0    14756 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/__init__.py
--rw-r--r--   0        0        0      170 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/config.py
--rw-r--r--   0        0        0     6637 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/game.py
--rw-r--r--   0        0        0     1728 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py
--rw-r--r--   0        0        0     1705 2023-06-27 11:15:28.542989 nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/model.py
--rw-r--r--   0        0        0      854 2023-06-27 11:15:28.546989 nonebot_plugin_chess-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 nonebot_plugin_chess-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1968 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/README.md
+-rw-r--r--   0        0        0    14793 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/config.py
+-rw-r--r--   0        0        0     6637 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/game.py
+-rw-r--r--   0        0        0     1728 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py
+-rw-r--r--   0        0        0     1705 2023-06-27 11:33:05.775656 nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/model.py
+-rw-r--r--   0        0        0      854 2023-06-27 11:33:05.779657 nonebot_plugin_chess-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 nonebot_plugin_chess-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_chess-0.4.0/LICENSE` & `nonebot_plugin_chess-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.4.0/README.md` & `nonebot_plugin_chess-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/__init__.py` & `nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from nonebot.rule import ArgumentParser, Rule
 from nonebot.typing import T_State
 
 require("nonebot_plugin_saa")
 require("nonebot_plugin_session")
 require("nonebot_plugin_userinfo")
 require("nonebot_plugin_datastore")
+require("nonebot_plugin_htmlrender")
 
 from nonebot_plugin_saa import Image, MessageFactory
 from nonebot_plugin_saa import __plugin_meta__ as saa_plugin_meta
 from nonebot_plugin_session import SessionIdType, SessionLevel
 from nonebot_plugin_session import __plugin_meta__ as session_plugin_meta
 from nonebot_plugin_session import extract_session
 from nonebot_plugin_userinfo import __plugin_meta__ as userinfo_plugin_meta
@@ -61,15 +62,15 @@
     homepage="https://github.com/noneplugin/nonebot-plugin-chess",
     config=Config,
     supported_adapters=supported_adapters,
     extra={
         "unique_name": "chess",
         "example": "@小Q 国际象棋人机lv5\ne2e4\n结束下棋",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.4.0",
+        "version": "0.4.1",
     },
 )
 
 
 parser = ArgumentParser("chess", description="国际象棋")
 group = parser.add_mutually_exclusive_group()
 group.add_argument("-e", "--stop", "--end", action="store_true", help="停止下棋")
```

### Comparing `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/game.py` & `nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py` & `nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/migrations/62899ffdd34f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.4.0/nonebot_plugin_chess/model.py` & `nonebot_plugin_chess-0.4.1/nonebot_plugin_chess/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chess-0.4.0/pyproject.toml` & `nonebot_plugin_chess-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_chess"
-version = "0.4.0"
+version = "0.4.1"
 description = "Nonebot2 国际象棋插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-chess"
 repository = "https://github.com/noneplugin/nonebot-plugin-chess"
```

### Comparing `nonebot_plugin_chess-0.4.0/PKG-INFO` & `nonebot_plugin_chess-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chess
-Version: 0.4.0
+Version: 0.4.1
 Summary: Nonebot2 国际象棋插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-chess
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

