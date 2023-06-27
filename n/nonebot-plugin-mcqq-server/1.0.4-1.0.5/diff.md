# Comparing `tmp/nonebot_plugin_mcqq_server-1.0.4.tar.gz` & `tmp/nonebot_plugin_mcqq_server-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mcqq_server-1.0.4.tar", last modified: Mon Jun 26 18:53:42 2023, max compression
+gzip compressed data, was "nonebot_plugin_mcqq_server-1.0.5.tar", last modified: Tue Jun 27 05:44:02 2023, max compression
```

## Comparing `nonebot_plugin_mcqq_server-1.0.4.tar` & `nonebot_plugin_mcqq_server-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:53:42.946040 nonebot_plugin_mcqq_server-1.0.4/
--rw-rw-rw-   0        0        0     1086 2022-09-08 17:56:17.000000 nonebot_plugin_mcqq_server-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      275 2023-06-26 18:53:42.945539 nonebot_plugin_mcqq_server-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 18:53:42.934029 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/
--rw-rw-rw-   0        0        0     3759 2023-06-26 18:51:48.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/__init__.py
--rw-rw-rw-   0        0        0      420 2023-02-25 09:44:03.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/config.py
--rw-rw-rw-   0        0        0     4331 2023-06-26 18:45:55.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:53:42.943537 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/
--rw-rw-rw-   0        0        0      275 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 18:53:42.946040 nonebot_plugin_mcqq_server-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-06-26 18:53:38.000000 nonebot_plugin_mcqq_server-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:44:02.315196 nonebot_plugin_mcqq_server-1.0.5/
+-rw-rw-rw-   0        0        0     1086 2022-09-08 17:56:17.000000 nonebot_plugin_mcqq_server-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      275 2023-06-27 05:44:02.314194 nonebot_plugin_mcqq_server-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 05:44:02.302185 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server/
+-rw-rw-rw-   0        0        0     4307 2023-06-27 05:43:09.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server/__init__.py
+-rw-rw-rw-   0        0        0      698 2023-06-27 04:51:00.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server/config.py
+-rw-rw-rw-   0        0        0     2839 2023-06-27 05:16:35.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:44:02.312193 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-06-27 05:44:02.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-27 05:44:02.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 05:44:02.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-27 05:44:02.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 05:44:02.000000 nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 05:44:02.315196 nonebot_plugin_mcqq_server-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-06-27 05:43:58.000000 nonebot_plugin_mcqq_server-1.0.5/setup.py
```

### Comparing `nonebot_plugin_mcqq_server-1.0.4/LICENSE` & `nonebot_plugin_mcqq_server-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/__init__.py` & `nonebot_plugin_mcqq_server-1.0.5/nonebot_plugin_mcqq_server/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+from pathlib import Path
 from nonebot import get_driver, on_message, on_command
 from nonebot.adapters.onebot.v11 import (
     Bot,
     Event,
     MessageEvent,
     GroupMessageEvent,
     GROUP_ADMIN,
     GROUP_OWNER
     )
 from nonebot.permission import SUPERUSER
 from nonebot_plugin_guild_patch import GuildMessageEvent
-from nonebot.rule import to_me
 from nonebot.log import logger
-
+from mcrcon import MCRcon,MCRconException
+import time
 import asyncio
 
-from pathlib import Path
-from .utils import (
+from .config import (
     group_list,
     guild_list,
     mc_log_path,
     mcrcon_password,
     mcrcon_port
     )
-from .utils import mcrcon_connect, mc_translate, log_to_dict
-
+from .utils import mc_translate, log_to_dict
 
 driver = get_driver()
 
 switch = False
 
 async def set_switch_rule(bot:Bot,event:MessageEvent, permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,):
     if event.to_me and await permission(bot,event):
@@ -76,38 +75,53 @@
 receive = on_message(rule = set_switch_rule, priority = 10, block = True)
 
 log = Path(mc_log_path) / "latest.log"
 if log.exists():
     logger.success(f"已找到 {log}")
     receive.append_handler(MC_TO_QQ)
     driver.on_bot_connect(MC_TO_QQ)
-    mcr = asyncio.run(mcrcon_connect("127.0.0.1", mcrcon_password, mcrcon_port))
 else:
     logger.error(f"mc_log_path 地址设置错误，{log} 不存在。")
 
+mcr = MCRcon("127.0.0.1", mcrcon_password, mcrcon_port)
 
-# 定义CUSTOMER权限
+async def QQ_TO_MC(event: Event):
+    global mcrcon_connect_is_running
+    if mcrcon_connect_is_running:
+        return
+    global mcr
+    timeout = time.time() + 30
+    while time.time() < timeout:
+        try:
+            mcr.command(mc_translate(event))
+            break
+        except (OSError, MCRconException) as e:
+            logger.error(f"信息发送失败：{e}")
+            await mcrcon_connect(mcr)
+
+mcrcon_connect_is_running = False
+
+async def mcrcon_connect(mcr:MCRcon):
+    global mcrcon_connect_is_running
+    mcrcon_connect_is_running = True
+    try:
+        mcr.connect()
+        mcrcon_connect_is_running = False
+        logger.success("与 MCRcon 连接成功！")
+    except (OSError, ConnectionRefusedError) as e:
+        logger.info(f"与 MCRcon 连接失败，正在重新连接...{e}")
+        await asyncio.sleep(3)
+        await mcrcon_connect(mcr)
 
 async def CUSTOMER(event: MessageEvent) -> bool:
     if isinstance(event,GroupMessageEvent):
         return event.group_id in group_list
     if isinstance(event,GuildMessageEvent):
         for guild in guild_list:
             if event.guild_id == guild["guild_id"] and event.channel_id == guild["channel_id"]:
                 return True
         else:
             return False
     return False
 
-async def QQ_TO_MC(bot: Bot, event: Event):
-    msg = await mc_translate(bot, event)
-    global mcr
-    while True:
-        try:
-            mcr.command(msg)
-            break
-        except Exception as e:
-            logger.error(f"连接失效：{e}")
-            mcr = await mcrcon_connect("127.0.0.1", mcrcon_password, mcrcon_port)
-
-send = on_message(rule = lambda :switch, permission = CUSTOMER, priority = 10)
+send = on_message(rule = lambda :switch and not mcrcon_connect_is_running, permission = CUSTOMER, priority = 10)
 send.append_handler(QQ_TO_MC)
```

### Comparing `nonebot_plugin_mcqq_server-1.0.4/setup.py` & `nonebot_plugin_mcqq_server-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_mcqq_server',
-version='1.0.4',
+version='1.0.5',
 description='mcqq服主版',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_mcqq_server"]),
```

