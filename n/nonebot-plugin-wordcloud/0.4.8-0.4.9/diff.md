# Comparing `tmp/nonebot_plugin_wordcloud-0.4.8.tar.gz` & `tmp/nonebot_plugin_wordcloud-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wordcloud-0.4.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_wordcloud-0.4.9.tar", max compression
```

## Comparing `nonebot_plugin_wordcloud-0.4.8.tar` & `nonebot_plugin_wordcloud-0.4.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-03-19 14:26:31.768288 nonebot_plugin_wordcloud-0.4.8/LICENSE
--rw-r--r--   0        0        0     4501 2023-03-19 14:26:31.768288 nonebot_plugin_wordcloud-0.4.8/README.md
--rw-r--r--   0        0        0  8331636 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/SourceHanSans.otf
--rw-r--r--   0        0        0    16633 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/__init__.py
--rw-r--r--   0        0        0     2400 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/config.py
--rw-r--r--   0        0        0     3516 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/data_source.py
--rw-r--r--   0        0        0     1519 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/migrations/ee2869aa7c5a_init_db.py
--rw-r--r--   0        0        0     2030 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/migrations/f26008eae177_alter_not_null.py
--rw-r--r--   0        0        0     2453 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/migrations/f77200370a39_ob12.py
--rw-r--r--   0        0        0      887 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/model.py
--rw-r--r--   0        0        0     9487 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/schedule.py
--rw-r--r--   0        0        0     3586 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/utils.py
--rw-r--r--   0        0        0     1709 2023-03-19 14:26:31.840288 nonebot_plugin_wordcloud-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     5778 1970-01-01 00:00:00.000000 nonebot_plugin_wordcloud-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-27 10:46:51.580325 nonebot_plugin_wordcloud-0.4.9/LICENSE
+-rw-r--r--   0        0        0    12914 2023-06-27 10:46:51.580325 nonebot_plugin_wordcloud-0.4.9/README.md
+-rw-r--r--   0        0        0  8331636 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/SourceHanSans.otf
+-rw-r--r--   0        0        0    16806 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/__init__.py
+-rw-r--r--   0        0        0     2400 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/config.py
+-rw-r--r--   0        0        0     3516 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/data_source.py
+-rw-r--r--   0        0        0     1519 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/migrations/ee2869aa7c5a_init_db.py
+-rw-r--r--   0        0        0     2030 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/migrations/f26008eae177_alter_not_null.py
+-rw-r--r--   0        0        0     2453 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/migrations/f77200370a39_ob12.py
+-rw-r--r--   0        0        0      887 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/model.py
+-rw-r--r--   0        0        0     9487 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/schedule.py
+-rw-r--r--   0        0        0     3586 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/utils.py
+-rw-r--r--   0        0        0     1711 2023-06-27 10:46:51.652326 nonebot_plugin_wordcloud-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    14184 1970-01-01 00:00:00.000000 nonebot_plugin_wordcloud-0.4.9/PKG-INFO
```

### Comparing `nonebot_plugin_wordcloud-0.4.8/LICENSE` & `nonebot_plugin_wordcloud-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/SourceHanSans.otf` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/SourceHanSans.otf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/__init__.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_chatrecorder")
 require("nonebot_plugin_datastore")
 from nonebot_plugin_chatrecorder import get_messages_plain_text
 from nonebot_plugin_datastore.db import post_db_init
 
-from .config import plugin_config, plugin_data
+from .config import Config, plugin_config, plugin_data
 from .data_source import get_wordcloud
 from .schedule import schedule_service
 from .utils import (
     get_datetime_fromisoformat_with_timezone,
     get_datetime_now_with_timezone,
     get_mask_key,
     get_time_fromisoformat_with_timezone,
@@ -83,14 +83,18 @@
 /删除词云默认形状
 
 设置定时发送每日词云
 /词云每日定时发送状态
 /开启词云每日定时发送
 /开启词云每日定时发送 23:59
 /关闭词云每日定时发送""",
+    homepage="https://github.com/he0119/nonebot-plugin-wordcloud",
+    type="application",
+    supported_adapters={"~onebot.v11", "~onebot.v12"},
+    config=Config,
 )
 
 wordcloud = CommandGroup("词云")
 
 
 wordcloud_cmd = wordcloud.command(
     "main",
```

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/config.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/data_source.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/migrations/ee2869aa7c5a_init_db.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/migrations/ee2869aa7c5a_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/migrations/f26008eae177_alter_not_null.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/migrations/f26008eae177_alter_not_null.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/migrations/f77200370a39_ob12.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/migrations/f77200370a39_ob12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/model.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/schedule.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/schedule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/nonebot_plugin_wordcloud/utils.py` & `nonebot_plugin_wordcloud-0.4.9/nonebot_plugin_wordcloud/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.4.8/pyproject.toml` & `nonebot_plugin_wordcloud-0.4.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "nonebot-plugin-wordcloud"
-version = "0.4.8"
+version = "0.4.9"
 description = "适用于 NoneBot2 的词云插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-wordcloud"
 repository = "https://github.com/he0119/nonebot-plugin-wordcloud"
 documentation = "https://github.com/he0119/nonebot-plugin-wordcloud#readme"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
 nonebot-adapter-onebot = "^2.2.0"
 nonebot-plugin-chatrecorder = "^0.2.3"
 wordcloud = "^1.8.1"
 jieba = "^0.42.1"
 tzdata = "*"
 "backports.zoneinfo" = { version = "^0.2.1", python = "<3.9" }
 emoji = ">=1.6.3,<3.0.0"
-nonebot-plugin-apscheduler = "^0.2.0"
-nonebot-plugin-datastore = "^0.6.0a2"
+nonebot-plugin-apscheduler = "^0.3.0"
+nonebot-plugin-datastore = ">=0.6.0, <2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 pre-commit = "*"
 nonebug = "^0.3.1"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.1.0"
 pytest-mock = "^3.7.0"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.0"
 gevent = "^22.10.2"
 asyncpg = "^0.27.0"
 aiomysql = "^0.1.1"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_wordcloud"]
 adapters = [
```

