# Comparing `tmp/pymino-1.2.1.9.tar.gz` & `tmp/pymino-1.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.2.1.8\dist\.tmp-vnrwl428\pymino-1.2.1.9.tar", last modified: Fri Jun 23 15:03:29 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino\pymino\dist\.tmp-nqhf5s89\pymino-1.2.2.1.tar", last modified: Tue Jun 27 05:01:46 2023, max compression
```

## Comparing `pymino-1.2.1.9.tar` & `pymino-1.2.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 15:03:29.821707 pymino-1.2.1.9/
--rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.9/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-06-23 15:03:29.822203 pymino-1.2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 15:03:29.754747 pymino-1.2.1.9/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-23 15:02:32.000000 pymino-1.2.1.9/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:03:29.786003 pymino-1.2.1.9/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/account.py
--rw-rw-rw-   0        0        0   343766 2023-06-23 13:53:34.000000 pymino-1.2.1.9/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    19900 2023-06-23 13:18:55.000000 pymino-1.2.1.9/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25932 2023-06-23 15:02:14.000000 pymino-1.2.1.9/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   342510 2023-06-23 13:54:12.000000 pymino-1.2.1.9/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/console.py
--rw-rw-rw-   0        0        0    44088 2023-06-23 15:02:13.000000 pymino-1.2.1.9/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-06-23 11:30:38.000000 pymino-1.2.1.9/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:03:29.810795 pymino-1.2.1.9/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-06-22 03:04:45.000000 pymino-1.2.1.9/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-06-22 04:13:53.000000 pymino-1.2.1.9/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-06-23 12:31:19.000000 pymino-1.2.1.9/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:03:29.820715 pymino-1.2.1.9/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-06-23 12:42:05.000000 pymino-1.2.1.9/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.9/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10355 2023-06-23 13:30:36.000000 pymino-1.2.1.9/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:03:29.768661 pymino-1.2.1.9/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-06-23 15:03:29.000000 pymino-1.2.1.9/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-06-23 15:03:29.000000 pymino-1.2.1.9/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 15:03:29.000000 pymino-1.2.1.9/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-23 15:03:29.000000 pymino-1.2.1.9/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 15:03:29.000000 pymino-1.2.1.9/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-23 15:03:29.824188 pymino-1.2.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:01:46.488830 pymino-1.2.2.1/
+-rw-rw-rw-   0        0        0     1085 2023-06-27 02:23:25.000000 pymino-1.2.2.1/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-06-27 05:01:46.492798 pymino-1.2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-06-27 05:01:27.000000 pymino-1.2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 05:01:46.339534 pymino-1.2.2.1/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-27 02:44:49.000000 pymino-1.2.2.1/pymino/__init__.py
+-rw-rw-rw-   0        0        0    11011 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30258 2023-06-27 04:58:42.000000 pymino-1.2.2.1/pymino/bot.py
+-rw-rw-rw-   0        0        0    36835 2023-06-27 04:14:26.000000 pymino-1.2.2.1/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:01:46.385662 pymino-1.2.2.1/pymino/ext/
+-rw-rw-rw-   0        0        0      528 2023-06-27 04:04:07.000000 pymino-1.2.2.1/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11204 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   343766 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    19900 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25932 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   342510 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    44088 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:01:46.443198 pymino-1.2.2.1/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15640 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    70180 2023-06-27 04:58:30.000000 pymino-1.2.2.1/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-06-27 04:58:47.000000 pymino-1.2.2.1/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:01:46.481390 pymino-1.2.2.1/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10322 2023-06-27 02:23:25.000000 pymino-1.2.2.1/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:01:46.358382 pymino-1.2.2.1/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-06-27 05:01:46.000000 pymino-1.2.2.1/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1533 2023-06-27 05:01:46.000000 pymino-1.2.2.1/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 05:01:46.000000 pymino-1.2.2.1/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-06-27 05:01:46.000000 pymino-1.2.2.1/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 05:01:46.000000 pymino-1.2.2.1/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-27 05:01:46.513630 pymino-1.2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-06-27 04:33:02.000000 pymino-1.2.2.1/setup.py
```

### Comparing `pymino-1.2.1.9/LICENSE` & `pymino-1.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/PKG-INFO` & `pymino-1.2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.9
+Version: 1.2.2.1
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.9 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.2.1 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.9/README.md` & `pymino-1.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/__init__.py` & `pymino-1.2.2.1/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.1.9'
+__version__ = '1.2.2.1'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.1.9/pymino/bot.py` & `pymino-1.2.2.1/pymino/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from threading import Thread
 from typing import Optional, Union
 from time import perf_counter, time
 
 from .ext.console import *
 from .ext.entities import *
 from .ext.socket import WSClient
+from .ext.global_client import Global
 from .ext.account import Account
 from .ext.community import Community
 from .ext.utilities.request_handler import RequestHandler
 from .ext.utilities.generate import device_id as generate_device_id
 
-class Bot(WSClient):
+class Bot(WSClient, Global):
     """
     `Bot` - This is the main client.
 
     `**Parameters**``
     - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
     - `community_id` - The community id to use for the bot. `Defaults` to `None`.
     - `console_enabled` - Whether to enable the console. `Defaults` to `True`.
@@ -213,15 +214,15 @@
         community_id: Union[str, int] = None,
         console_enabled: bool = False,
         device_id: str = None,
         intents: bool = False,
         online_status: bool = False,
         proxy: str = None
         ):
-
+        
         self._debug:            bool = check_debugger()
         self._console_enabled:  bool = console_enabled
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
@@ -241,15 +242,15 @@
                                 )
         self.account:           Account = Account(
                                 session=self.request
                                 )
 
         if self.community_id:   self.set_community_id(community_id)
 
-        WSClient.__init__(self)
+        super().__init__()
 
 
     @property
     def debug(self) -> bool:
         """
         Whether or not debug mode is enabled.
 
@@ -601,14 +602,15 @@
                 )
 
         if not response:
             raise LoginFailed
 
         return self._run(response)
 
+
     def _run(self, response: dict) -> dict:
         """
         Processes the response from a successful login attempt and sets up the authenticated client.
 
         :param response: The response from the login attempt.
         :type response: dict
         :return: The response from the login attempt.
@@ -752,15 +754,16 @@
         except VerifyCommunityIdIsCorrect as e:
             raise VerifyCommunityIdIsCorrect from e
 
         self.community_id = community_id
         self.community.community_id = community_id
 
         return community_id
-    
+
+
     def ping(self) -> float:
         """
         Pings the server and returns the elapsed time in milliseconds.
         
         :return: The elapsed time in milliseconds.
         :rtype: float
```

### Comparing `pymino-1.2.1.9/pymino/client.py` & `pymino-1.2.2.1/pymino/ext/global_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1144 +1,177 @@
-from time import time
-from typing import Any, Callable, Optional, TypeVar, Union
-
-from .ext.entities import *
-from .ext import RequestHandler, Account, Community
-from .ext.utilities.generate import device_id as generate_device_id
+from .entities import *
+from .utilities.generate import *
+from typing import Any, Callable, TypeVar
 
 
 F = TypeVar("F", bound=Callable[..., Any])
 
-class Client:
-    """
-    `Client` - This is the main client.
-
-    `**Parameters**``
-    - `**kwargs` - any other parameters to use for the client.
-
-    - `device_id` - device id to use for the client.
-
-    - `proxy` - proxy string to use for the client.
-    
-    ----------------------------
-    Why use `Client` over `Bot`?
-
-    - Used for scripts rather than bots.
-    - Lightweight, does not utilize websocket.
-
-    ----------------------------
-    Do I have to be logged in to use `Client`?
-
-    - No, you do not have to be logged in to use `Client`.
-    - However, you will not be able to use any methods that require authentication.
-
-    `**NON-AUTH EXAMPLE**`
-    ```python
-    # This method does not require authentication, so it will work without logging in.    
-
-    from pymino import Client
-
-    client = Client()
-
-    print(f"Logged in: {client.is_authenticated}")
-
-    chat_id = client.community.fetch_object_id(link="https://aminoapps.com/p/123456789")
-
-    print(f"Chat ID: {chat_id}")
-    ```
-    ----------------------------
-
-    How do I login with `Client`?
-        - You can login with `Client` by using the `login` method.
-        
-    `**Login Example**`
-
-    ```python
-    from pymino import Client
-
-    client = Client()
-
-    client.login(email="email", password="password")
-
-    print(f"Logged in: {client.is_authenticated}")
-
-    # Output: Logged in: True
-    ```
-    ----------------------------
-    How can I utilize community methods with `Client`?
-        - First, you must set the community id.
-        - You can set the community id by using the `set_community_id` method
-        - Or the `fetch_community_id` method if you do not know the community id.
-
-    `**Community Example**`
-    ```python
-    from pymino import Client
-
-    client = Client()
-
-    client.login(email="email", password="password")
-
-    print(f"Logged in: {client.is_authenticated}")
-
-    client.fetch_community_id("http://aminoapps.com/c/CommunityName")
-    # Or
-    client.set_community_id(123456789)
-
-    print(f"Community ID has been set: {client.community_id}")
-    ```
-    ----------------------------
-    `**Community Methods**`
-    ```python
-    from pymino import Client
-
-    client = Client()
-
-    client.login(email="email", password="password")
-
-    client.fetch_community_id("http://aminoapps.com/c/CommunityName")
-
-    client.community.send_message(
-        chatId = "000000-0000-0000-0000-000000",
-        content = "Hello, world!"
-    ) # This will send in the community you set the community id for.
-
-    #Alternatively, you can use the community id as a parameter.
-    comId = client.fetch_community_id("http://aminoapps.com/c/CommunityName")
-    client.community.send_message(
-        chatId = "000000-0000-0000-0000-000000",
-        content = "Hello, world!",
-        comId = comId
-    )
-    ```
-
-    """
-    def __init__(self, **kwargs):
-        self._debug:            bool = check_debugger()
-        self._is_authenticated: bool = False
-        self._userId:           str = None
-        self._sid:              str = None
-        self._cached:           bool = False
-        self.cache:             Cache = Cache("cache")
-        self.community_id:      Optional[str] = kwargs.get("comId", kwargs.get("community_id"))
-        self.device_id:         Optional[str] = kwargs.get("device_id") or generate_device_id()
-        self.request:           RequestHandler = RequestHandler(
-                                self,
-                                proxy=kwargs.get("proxy")
-                                )
-        self.account:           Account = Account(
-                                session=self.request
-                                )
-        self.community:         Community = Community(
-                                bot=self,
-                                session=self.request,
-                                community_id=self.community_id
-                                )
-
-
-    @property
-    def debug(self) -> bool:
-        """
-        Whether or not debug mode is enabled.
-
-        :return: True if debug mode is enabled, False otherwise.
-        :rtype: bool
-
-        This property returns whether or not debug mode is enabled. Debug mode can be used to enable additional logging and
-        debug information during development.
-
-        **Note:** This property only returns the debug mode state and cannot be used to set the debug mode state. To set the
-        debug mode state, use the `self._debug` attribute directly.
-        """
-        return self._debug
-    
-
-    @debug.setter
-    def debug(self, value: bool) -> None:
-        """
-        Sets the debug mode state.
-
-        :param value: True to enable debug mode, False to disable it.
-        :type value: bool
-        :return: None
-
-        This setter sets the debug mode state. Debug mode can be used to enable additional logging and debug information
-        during development.
-
-        **Note:** This setter only sets the debug mode state and cannot be used to retrieve the debug mode state. To retrieve
-        the debug mode state, use the `self.debug` property.
-        """
-        self._debug = value
-
-
-    @property
-    def is_authenticated(self) -> bool:
-        """
-        Whether or not the client is authenticated.
-
-        :return: True if the client is authenticated, False otherwise.
-        :rtype: bool
-
-        This property returns whether or not the client is authenticated. The client is authenticated after logging in to
-        Amino and receiving a valid session ID.
-
-        **Note:** This property only returns the authentication state and cannot be used to set the authentication state. To
-        set the authentication state, use the `self._is_authenticated` attribute directly.
-        """
-        return self._is_authenticated
-    
-
-    @is_authenticated.setter
-    def is_authenticated(self, value: bool) -> None:
-        """
-        Sets the authentication state of the client.
-
-        :param value: True to authenticate the client, False to deauthenticate it.
-        :type value: bool
-        :return: None
-
-        This setter sets the authentication state of the client. The client is authenticated after logging in to Amino and
-        receiving a valid session ID.
-
-        **Note:** This setter only sets the authentication state and cannot be used to retrieve the authentication state. To
-        retrieve the authentication state, use the `self.is_authenticated` property.
-        """
-        self._is_authenticated = value
-
-
-    @property
-    def userId(self) -> str:
-        """
-        The ID of the user associated with the client.
-
-        :return: The ID of the user.
-        :rtype: str
-
-        This property returns the ID of the user associated with the client. The user ID is set when the client logs in to
-        Amino, and can be used to make API calls related to the user, such as retrieving the user's profile or posts.
-
-        **Note:** This property only returns the user ID and cannot be used to set the user ID. To set the user ID, use the
-        `self._userId` attribute directly.
-        """
-        return self._userId
-
-
-    @userId.setter
-    def userId(self, value: str) -> None:
-        """
-        Sets the ID of the user associated with the client.
-
-        :param value: The ID of the user to set.
-        :type value: str
-        :return: None
-
-        This setter sets the ID of the user associated with the client. The user ID is used to make API calls related to the
-        user, such as retrieving the user's profile or posts.
-
-        **Note:** This setter only sets the user ID and cannot be used to retrieve the user ID. To retrieve the user ID, use
-        the `self.userId` property.
-        """
-        self._userId = value
-
-        
-    @property
-    def sid(self) -> str:
-        """
-        The session ID of the client.
-
-        :return: The session ID.
-        :rtype: str
-
-        This property returns the session ID of the client. The session ID is set when the client logs in to Amino, and is
-        used to make authenticated API calls, such as posting messages or retrieving user information.
-
-        **Note:** This property only returns the session ID and cannot be used to set the session ID. To set the session ID,
-        use the `self._sid` attribute directly.
-        """
-        return self._sid
-
-
-    @sid.setter
-    def sid(self, value: str) -> None:
-        """
-        Sets the session ID of the client.
-
-        :param value: The session ID to set.
-        :type value: str
-        :return: None
-
-        This setter sets the session ID of the client. The session ID is used to make authenticated API calls, such as
-        posting messages or retrieving user information.
-
-        **Note:** This setter only sets the session ID and cannot be used to retrieve the session ID. To retrieve the session
-        ID, use the `self.sid` property.
-        """
-        self._sid = value
+class Global:
+    def __init__(self) -> None:
+        pass
 
 
     def authenticated(func: F) -> F:
         """
-        A decorator that ensures the user is authenticated before running the decorated function.
-
-        :param func: The function to be decorated.
-        :type func: Callable
-        :raises LoginRequired: If the user is not authenticated.
-        :return: The result of calling the decorated function.
-        :rtype: Any
-
-        **Example usage:**
-
-        >>> client = Client()
-        >>> client.login(email="example@example.com", password="password")
-
-        >>> @authenticated
-        >>> def my_function(self):
-        >>>     # Function code
+        A decorator that checks if the client is authenticated.
+        
+        :param func: The function to decorate.
+        :type func: F
+        :return: The decorated function.
+        :rtype: F
+        
+        This decorator is used to check if the client is authenticated.
+        If the client is not authenticated, a `LoginRequired` exception
+        will be raised.
         """
         def wrapper(*args, **kwargs) -> Any:
             try:
                 if not args[0].is_authenticated:
                     raise LoginRequired
                 return func(*args, **kwargs)
             except AttributeError:
                 raise LoginRequired
         return wrapper
 
 
-    def fetch_community_id(self, community_link: str, set_community_id: Optional[bool] = True) -> int:
+    def make_request(self, method: str, url: str, data: dict = None) -> dict:
         """
-        Fetches the community ID associated with the provided community link.
-
-        :param community_link: The community link for which to fetch the ID.
-        :type community_link: str
-        :param set_community_id: Whether or not to set the fetched community ID on the client instance. Defaults to True.
-        :type set_community_id: Optional[bool]
-        :return: The community ID associated with the provided community link.
-        :rtype: int
-
-        The function first checks if the community ID for the provided community link is already present in the cache.
-        If not, it fetches the community ID from the server using the provided community link. It then stores the community
-        ID in the cache for future use.
-
-        If the `set_community_id` parameter is set to True, the function also sets the community ID on the client instance
-        for future API calls.
-
-        If the provided community link is not found on the server, the function raises a CommunityNotFound exception.
-
-        **Note:** The community ID is required for making API calls related to a specific community, such as posting or
-        retrieving posts. It is recommended to use this function if you do not already know the community ID.
-        """
-        KEY = str((community_link, "comId"))
-        if not self.cache.get(KEY):
-            self.cache.set(KEY, CCommunity(self.request.handler(
-                method="GET", url=f"/g/s/link-resolution?q={community_link}")
-                ).comId)
-            
-        community_id = self.cache.get(KEY)
-
-        if set_community_id:
-            self.set_community_id(community_id)
-
-        return community_id
-
-
-    def set_community_id(self, community_id: Union[str, int]) -> int:
-        """
-        Sets the community ID on the client instance and the Community object.
-
-        :param community_id: The community ID to set.
-        :type community_id: Union[str, int]
-        :return: The community ID that was set.
-        :rtype: int
-
-        The function first checks if the provided community ID is not None and not already an integer. If it is a string,
-        it converts it to an integer.
-
-        If the community ID cannot be verified, the function raises a VerifyCommunityIdIsCorrect exception.
-
-        The function then sets the community ID on the client instance and the Community object for future API calls.
-
-        **Note:** The community ID is required for making API calls related to a specific community, such as posting or
-        retrieving posts. It is recommended to use the `fetch_community_id` function if you do not already know the
-        community ID.
-        """
-        try:
-            if community_id is not None and not isinstance(community_id, int):
-                community_id = int(community_id)
-        except VerifyCommunityIdIsCorrect as e:
-            raise VerifyCommunityIdIsCorrect from e
-
-        self.community_id = community_id
-        self.community.community_id = community_id
-
-        return community_id
-
-
-    def authenticate(self, email: str, password: str, device_id: str=None) -> dict:
-        """
-        Authenticates the bot with the provided email and password.
-
-        :param email: The email to use to log in.
-        :type email: str
-        :param password: The password to use to log in.
-        :type password: str
-        :param device_id: The device id to use to log in. Defaults to None.
-        :type device_id: Optional[str]
-        :return: A dictionary representing the server response.
-        :rtype: dict
-        :raises: `APIError` if the API response code is not 200.
-        """
-        if device_id:
-            self.device_id = device_id
-
-        return ApiResponse(self.request.handler(
-            method="POST",
-            url = "/g/s/auth/login",
-            data = {
-                "secret": f"0 {password}",
-                "clientType": 100,
-                "systemPushEnabled": 0,
-                "timestamp": int(time() * 1000),
-                "locale": "en_US",
-                "action": "normal",
-                "bundleID": "com.narvii.master",
-                "timezone": -480,
-                "deviceID": self.device_id,
-                "email": email,
-                "v": 2,
-                "clientCallbackURL": "narviiapp://default"
-                }
-            )).json()
-
-
-    def _login_handler(self, email: str, password: str, device_id: str=None, use_cache: bool=True) -> dict:
-        """
-        Authenticates the user with the provided email and password.
-
-        :param email: The email address associated with the account.
-        :type email: str
-        :param password: The password for the account.
-        :type password: str
-        :param device_id: The device ID associated with the account. Defaults to None.
-        :type device_id: Optional[str]
-        :param use_cache: Whether or not to use cached login credentials. Defaults to True.
-        :type use_cache: bool
-        :return: A dictionary containing the login response from the server.
-        :rtype: dict
+        Makes a request to the API.
         
-        The function first checks if cached login credentials are available for the provided email. If so, it uses the cached
-        session ID and device ID to fetch the account details from the server. If the server returns an exception, it falls
-        back to authenticating with the provided email and password, and the device ID from the cache.
-
-        If no cached credentials are available, the function authenticates with the provided email and password, and the
-        provided or default device ID.
-
-        Finally, the function sets the email and password on the request object for future API calls.
-
-        **Note:** This function should not be called directly. Instead, use the `login` function to authenticate the user.
-        """
-        if use_cache and cache_exists(email=email):
-            cached = fetch_cache(email=email)
-
-            self.sid: str = cached[0]
-            self.request.sid: str = cached[0]
-            self.userId: str = parse_auid(cached[0])
-
-            try:
-                response: dict = self.fetch_account()
-            except Exception:
-                response: dict = self.authenticate(
-                    email=email,
-                    password=password,
-                    device_id=cached[1]
-                    )
-
-        else:
-            self.sid = None
-            self._cached = True
-            response: dict = self.authenticate(
-                email=email,
-                password=password,
-                device_id=device_id
-                )
-
-        for key, value in {"email": email, "password": password}.items():
-            setattr(self.request, key, value)            
-
-        return response
-
-
-    def login(
-        self,
-        email: Optional[str] = None,
-        password: Optional[str] = None,
-        sid: Optional[str] = None,
-        device_id: Optional[str] = None,
-        use_cache: bool = True
-        ) -> None:
-        """
-        Logs in to the client using the provided credentials.
-
-        :param email: The email address associated with the account. Defaults to None.
-        :type email: Optional[str]
-        :param password: The password for the account. Defaults to None.
-        :type password: Optional[str]
-        :param sid: The session ID for the account. Defaults to None.
-        :type sid: Optional[str]
-        :param device_id: The device ID associated with the account. Defaults to None.
-        :type device_id: Optional[str]
-        :param use_cache: Whether or not to use cached login credentials. Defaults to True.
-        :type use_cache: bool
-        :raises MissingEmailPasswordOrSid: If no email, password or sid is provided.
-        :raises LoginFailed: If login failed.
-        :return: None
-        :rtype: None
-
-        **Example usage:**
-
-        >>> client = Client()
-        >>> client.login(email="example@example.com", password="password")
-        """
-        if not sid and not email and not password:
-            raise MissingEmailPasswordOrSid
-
-        if sid:
-            self.sid = sid
-            self.request.sid = sid
-            self.userId = parse_auid(sid)
-            response = self.fetch_account()
-        else:
-            response = self._login_handler(
-                email=email,
-                password=password,
-                device_id=device_id,
-                use_cache=use_cache
-                )
-
-        if not response:
-            raise LoginFailed
-
-        return self._run(response)
-
-
-    def run(
-        self,
-        email: Optional[str] = None,
-        password: Optional[str] = None,
-        sid: Optional[str] = None,
-        device_id: Optional[str] = None,
-        use_cache: bool = True
-    ) -> None:
-        """
-        Logs in to the client and starts running it. 
-
-        If authentication is successful, the bot will be logged in and the client will be ready to use.
-
-        :param email: The email to use to log in. Defaults to None.
-        :type email: str, optional
-        :param password: The password to use to log in. Defaults to None.
-        :type password: str, optional
-        :param sid: The sid to use to log in. Defaults to None.
-        :type sid: str, optional
-        :param device_id: The device id to use to log in. Defaults to None.
-        :type device_id: str, optional
-        :param use_cache: Whether to use the cache to retrieve the sid. Defaults to True.
-        :type use_cache: bool, optional
-        :raises MissingEmailPasswordOrSid: If email, password, or sid is missing.
-        :raises LoginFailed: If authentication failed.
-        :return: None.
-        :rtype: None
-
-        **Example usage:**
-
-        >>> client = Client()
-        >>> client.run(email="example@example.com", password="password")
-        """
-        return self.login(email=email, password=password, sid=sid, device_id=device_id, use_cache=use_cache)
-
-
-    def _run(self, response: dict) -> dict:
-        """
-        Processes the response from a successful login attempt and sets up the authenticated client.
-
-        :param response: The response from the login attempt.
-        :type response: dict
-        :return: The response from the login attempt.
+        :param method: The HTTP method to use.
+        :type method: str
+        :param url: The URL to make the request to.
+        :type url: str
+        :param data: The data to send with the request.
+        :type data: dict
+        :return: The response from the request.
         :rtype: dict
-
-        This method is called internally by the `login` and `run` methods after a successful login attempt.
-        It sets up the authenticated client by parsing the response, initializing some client properties,
-        and caching the login credentials if applicable.
-
-        If the `debug` property of the client instance is `True`, this method prints a message to the console
-        confirming that the client is now authenticated.
-
-        **Example usage:**
-
-        >>> client = Client()
-        >>> response = client.authenticate(email="example@example.com", password="password")
-        >>> client._run(response)
-        """
-        if response["api:statuscode"] != 0: input(response), exit()
-
-        if not hasattr(self, "profile"): 
-            self.profile: UserProfile = UserProfile(response)
-
-        if not self.sid:
-            self.sid: str = response["sid"]
-
-        self.userId: str = self.profile.userId
-        self.community.userId: str = self.userId
-        self.request.sid: str = self.sid
-        self.request.userId: str = self.userId
-        self.is_authenticated: bool = True
-
-        if hasattr(self.request, "email") and self._cached:
-            cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
-
-        if self.debug:
-            print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
-
-        return response
-
-
-    def fetch_object_id(self, link: str) -> str:
-        """
-        Fetches the object ID given a link to the object.
-
-        :param link: The link to the object.
-        :type link: str
-        :raises NotLoggedIn: If the user is not logged in.
-        :raises MissingCommunityId: If the community ID is missing.
-        :return: The ID of the object.
-        :rtype: str
-
-        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
-        The method caches the object ID for faster access in future calls.
-
-        **Example usage:**
-
-        >>> object_id = client.community.fetch_object_id(link="https://aminoapps.com/p/w2Fs6H")
-        >>> print(object_id)
-        """
-
-        KEY = str((link, "OBJECT_ID"))
-        if not self.cache.get(KEY):
-            self.cache.set(KEY, self.request.handler(
-                method = "GET",
-                url = f"/g/s/link-resolution?q={link}"
-                ))
-        return LinkInfo(self.cache.get(KEY)).objectId
-    
-
-    def fetch_object_info(self, link: str) -> LinkInfo:
-        """
-        Fetches information about an object given its link.
-
-        :param link: The link to the object.
-        :type link: str
-        :raises NotLoggedIn: If the user is not logged in.
-        :raises MissingCommunityId: If the community ID is missing.
-        :return: A LinkInfo object containing information about the object.
-        :rtype: LinkInfo
-
-        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
-        The method caches the object information for faster access in future calls.
-
-        `LinkInfo`:
-
-        - `data`: The raw response data from the API.
-        - `linkInfoV2`: The link information data.
-        - `path`: The path of the object.
-        - `extensions`: The extensions data.
-        - `objectId`: The ID of the object.
-        - `shareURLShortCode`: The short code of the share URL.
-        - `targetCode`: The target code.
-        - `ndcId`: The NDC ID.
-        - `comId`: The community ID.
-        - `fullPath`: The full path of the object.
-        - `shortCode`: The short code of the object.
-        - `objectType`: The type of the object.
-
-        **Example usage:**
-
-        >>> object_info = client.community.fetch_object_info(link="https://aminoapps.com/p/w2Fs6H")
-        >>> print(object_info.objectId)
-        """
-
-        KEY = str((link, "OBJECT_INFO"))
-        if not self.cache.get(KEY):
-            self.cache.set(KEY, self.request.handler(
-                method = "GET",
-                url = f"/g/s/link-resolution?q={link}"
-                ))
-        return LinkInfo(self.cache.get(KEY))
-    
-    @authenticated
-    def disconnect_google(self, password: str) -> dict:
-        """
-        Disconnects the user's Google account from their account on Amino.
-
-        :param password: The user's account password.
-        :type password: str
-        :return: A dictionary containing the server response.
-        :rtype: dict
-
-        If the client is authenticated, the function sends a POST request to the server to disconnect the user's Google
-        account. The request includes the client's device ID, the user's account password, and other required parameters.
-
-        The function returns a dictionary containing the server response.
-
-        **Note:** This function can be used to disconnect the user's Google account from their Amino account, for example if
-        the user wants to use a different Google account or does not want to use Google to sign in anymore.
+        
+        This method is used to make requests to the API.
+        
+        Example usage:
+        
+        >>> client.make_request(
+            ...     method = "GET",
+            ...     url = "/g/s/user-profile/0000-000000-000000-0000-000000"
+            ... )
+            
+        This will make a GET request to the URL `/g/s/user-profile/0000-000000-000000-0000-000000`.
         """
         return self.request.handler(
-            method="POST",
-            url="/g/s/auth/disconnect",
-            data={
-                "deviceID": self.device_id,
-                "secret": f"0 {password}",
-                "type": 30,
-                "timestamp": int(time() * 1000),
-                }
-            )
-
-
-    @authenticated
-    def logout(self) -> None:
-        """
-        Logs out the user by clearing the session ID and user ID on the client instance.
-
-        :return: None
-        :rtype: None
-        :raises LoginRequired: If the authentication fails.
-
-        This function first checks if the client is authenticated by checking for a valid session ID. If the client is not
-        authenticated, the function raises a `LoginRequired` exception.
-
-        If the client is authenticated, the function clears the session ID and user ID on the client instance, as well as
-        other related attributes. This effectively logs out the user.
-
-        The function returns None.
-
-        **Note:** After calling this function, the client will no longer be authenticated and will need to log in again to
-        make authenticated API calls.
-        """
-        for key in ["sid", "userId", "community.userId", "request.sid", "request.userId", "is_authenticated"]:
-            setattr(self, key, None)
-        return None
-
-
-    @authenticated
-    def join_community(self, community_id: int, invitationId = None) -> ApiResponse:
-        """
-        Joins the user to a community with the provided community ID.
-
-        :param community_id: The ID of the community to join.
-        :type community_id: int
-        :param invitationId: The ID of the invitation link.
-        :type invitationId: str
-        :return: An ApiResponse object containing the server response.
-        :rtype: ApiResponse
-        :raises LoginRequired: If the user is not logged in.
-
-        This function first checks if the client is logged in by checking for a valid session ID. If not, it raises a
-        LoginRequired exception.
-
-        If the client is logged in, the function sends a POST request to the server to join the specified community.
-        The request includes the client's session ID and the ID of the community to join.
-
-        The function returns an ApiResponse object containing the server response.
-
-        **Note:** This function can be used to join the user to a community with the provided community ID. Once joined,
-        the user can make API calls related to the community, such as posting or retrieving posts.
-        """
-        data = {"timestamp": int(time() * 1000)}
-        if invitationId:
-            data["invitationId"] = invitationId
-
-        return ApiResponse(
-            self.request.handler(
-                method="POST",
-                url=f"/x{community_id}/s/community/join",
-                data = data
-        ))
-
-    @authenticated
-    def leave_community(self, community_id: int) -> ApiResponse:
-        """
-        Leaves the user from a community with the provided community ID.
-
-        :param community_id: The ID of the community to leave.
-        :type community_id: int
-        :return: An ApiResponse object containing the server response.
-        :rtype: ApiResponse
-        :raises LoginRequired: If the user is not logged in.
-
-        This function first checks if the client is logged in by checking for a valid session ID. If not, it raises a
-        LoginRequired exception.
-
-        If the client is logged in, the function sends a POST request to the server to leave the specified community.
-        The request includes the client's session ID and the ID of the community to leave.
-
-        The function returns an ApiResponse object containing the server response.
+            method = method,
+            url = url,
+            data = data
+        )
 
-        **Note:** This function can be used to leave the user from a community with the provided community ID. Once left,
-        the user will no longer have access to the community and will not be able to make API calls related to the community.
-        """
-        return ApiResponse(self.request.handler(
-            method="POST",
-            url=f"/x{community_id}/s/community/leave"
-            ))
 
     def fetch_user(self, userId: str) -> UserProfile:
         """
-        Fetches the user profile of the user with the provided user ID.
-
-        :param userId: The ID of the user whose profile to fetch.
+        Fetches a user's profile.
+        
+        :param userId: The ID of the user to fetch.
         :type userId: str
-        :return: A UserProfile object representing the user profile.
+        :return: The user's profile.
         :rtype: UserProfile
-
-        This function sends a GET request to the server to fetch the user profile of the user with the provided user ID.
-        The request includes the ID of the user to fetch.
-
-        The function returns a UserProfile object representing the user profile. The UserProfile object contains attributes
-        such as the user's ID, nickname, avatar URL, and other profile information.
-
-        **Note:** This function can be used to fetch the user profile of a user on Amino. The user profile can be used to
-        display information about the user or to make API calls related to the user, such as retrieving the user's posts or
-        other information.
-        """
-        return UserProfile(self.request.handler(
-            method="GET",
-            url=f"/g/s/user-profile/{userId}"
-            ))
-
-
-    def fetch_community(self, community_id: int) -> CCommunity:
-        """
-        Fetches the community information for the community with the provided community ID.
-
-        :param community_id: The ID of the community to fetch.
-        :type community_id: int
-        :return: A CCommunity object representing the community information.
-        :rtype: CCommunity
-
-        This function sends a GET request to the server to fetch the community information for the community with the
-        provided community ID. The request includes the ID of the community to fetch.
-
-        The function returns a CCommunity object representing the community information. The CCommunity object contains
-        attributes such as the members count, the community's layout, and other community information.
-
-        **Note:** This function can be used to fetch the community information for a community on Amino. The community
-        information can be used to display information about the community such as the community's name, description, and
-        other information.
-        """
-        return CCommunity(self.request.handler(
-            method="GET",
-            url=f"/g/s-x{community_id}/community/info"
-            ))
-
-    @authenticated
-    def joined_communities(self) -> CCommunityList:
-        """
-        Retrieves the list of communities that the authenticated user has joined.
-
-        :return: The list of communities.
-        :rtype: CCommunityList
-
-        This method returns the list of communities that the authenticated user has joined. The list includes information
-        such as the community ID, name, description, and theme.
-
-        **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
-        be raised.
-        """
-        return CCommunityList(self.request.handler(
-            method="GET",
-            url="/g/s/community/joined"
-            ))
-
-    @authenticated
-    def join_chat(self, chatId: str) -> ApiResponse:
-        """
-        Joins the authenticated user to a chat thread.
-
-        :param chatId: The ID of the chat thread to join.
-        :type chatId: str
-        :return: The API response.
-        :rtype: ApiResponse
-
-        This method joins the authenticated user to a chat thread. The user must be a member of the community that the chat
-        thread belongs to in order to join the thread.
-
-        **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
-        be raised.
-        """
-        return ApiResponse(self.request.handler(
-            method="POST",
-            url=f"/g/s/chat/thread/{chatId}/member/{self.userId}"
-            ))
-
-    @authenticated
-    def leave_chat(self, chatId: str) -> ApiResponse:
-        """
-        Removes the authenticated user from a chat thread.
-
-        :param chatId: The ID of the chat thread to leave.
-        :type chatId: str
-        :return: The API response.
-        :rtype: ApiResponse
-
-        This method removes the authenticated user from a chat thread. The user must be a member of the chat thread in order
-        to leave it.
-
-        **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
-        be raised.
-        """
-        return ApiResponse(self.request.handler(
-            method="DELETE",
-            url=f"/g/s/chat/thread/{chatId}/member/{self.userId}"
-            ))
-
-    def register(self, email: str, password: str, username: str, verificationCode: str) -> Authenticate:
-        """
-        Registers a new account with the provided email, password, username, and verification code.
-
-        :param email: The email address to register the account with.
-        :type email: str
-        :param password: The password to use for the account.
-        :type password: str
-        :param username: The username to use for the account.
-        :type username: str
-        :param verificationCode: The verification code sent to the email address for account activation.
-        :type verificationCode: str
-        :return: An `Authenticate` object containing the authenticated user's session ID, user ID, and community user ID.
-        :rtype: Authenticate
-
-        This method registers a new account with the provided email, password, username, and verification code. The
-        verification code is sent to the email address for account activation. The method returns an `Authenticate` object
-        containing the authenticated user's session ID and user ID.
-        """
-        return self.account.register(email=email, password=password, username=username, verificationCode=verificationCode)
-
-    @authenticated
-    def delete_request(self, email: str, password: str) -> ApiResponse:
-        """
-        Sends a request to delete the authenticated user's account.
-
-        :param email: The email address associated with the account.
-        :type email: str
-        :param password: The password for the account.
-        :type password: str
-        :return: An `ApiResponse` object containing the server's response to the delete request.
-        :rtype: ApiResponse
-
-        This method sends a request to delete the authenticated user's account. The email and password parameters are used to
-        authenticate the request. The method returns an `ApiResponse` object containing the server's response to the delete
-        request.
-        """
-        return self.account.delete_request(email=email, password=password)
-
-    @authenticated
-    def delete_request_cancel(self, email: str, password: str) -> ApiResponse:
-        """
-        Cancels a previously requested account deletion for the authenticated user.
-
-        :param email: The email address associated with the account.
-        :type email: str
-        :param password: The password for the account.
-        :type password: str
-        :return: An `ApiResponse` object containing the server's response to the delete request cancellation request.
-        :rtype: ApiResponse
-
-        This method cancels a previously requested account deletion for the authenticated user. The email and password
-        parameters are used to authenticate the request. The method returns an `ApiResponse` object containing the server's
-        response to the delete request cancellation request.
-        """
-        return self.account.delete_request_cancel(email=email, password=password)
-
-    def check_device(self, device_id: str) -> ApiResponse:
-        """
-        Checks if the given device ID is valid.
-
-        :param device_id: The ID of the device to check.
-        :type device_id: str
-        :return: An `ApiResponse` object containing the server's response to the device check request.
-        :rtype: ApiResponse
-
-        This method checks if the device ID is valid. The device ID is
-        passed as a string argument. The method calls the `check_device` method of the `account` object with the
-        `deviceId` parameter set to the given device ID. The result is an `ApiResponse` object that contains the server's
-        response to the device check request.
-
-        The method returns the `ApiResponse` object obtained from calling the `check_device` method of the `account`
-        object. The response will return a `0` status code if the device ID is valid.
-        """
-        return self.account.check_device(deviceId=device_id)
-
-
-    def fetch_account(self) -> dict:
-        """
-        Fetches the account information for the authenticated user.
-
-        :return: A dictionary containing the user's account information.
-        :rtype: dict
-
-        This method fetches the account information for the authenticated user. The account information includes
-        the user's username, email address, and other relevant details. The method calls the `UserProfile` object's
-        `handler` method with the `method` parameter set to `GET` and the `url` parameter set to the user profile endpoint.
-        The result is an `ApiResponse` object that contains the user's profile information.
-
-        The method then calls the `handler` method of the `request` object with the `method` parameter set to `GET`
-        and the `url` parameter set to the account endpoint. The result is an `ApiResponse` object that contains the
-        user's account information in JSON format.
-
-        The method returns a dictionary containing the user's account information.
-        """
-        self.profile: UserProfile = UserProfile(
-            self.request.handler(
-                method="GET",
-                url=f"/g/s/user-profile/{self.userId}"
-                ))
         
-        return ApiResponse(self.request.handler(method="GET", url="/g/s/account")).json()
-
-
-    @authenticated
-    def upload_image(self, image: str) -> str:
-        """
-        Uploads an image to amino servers.
-
-        :param image: The base64-encoded image data.
-        :type image: str
-        :return: The URL of the uploaded image.
-        :rtype: str
-
-        This method uploads an image to amino servers. The image data is passed as a string argument. The method calls the
-        `upload_image` method of the `account` object with the `image` parameter set to the given image data. The result is
-        a `mediaValue` object that contains the URL of the uploaded image.
-
-        The method returns the URL of the uploaded image.
-        """
-        return self.account.upload_image(image=image).mediaValue
-
-
-    @authenticated
-    def fetch_profile(self) -> UserProfile:
-        """
-        Fetches the user profile of the authenticated user.
-
-        :return: A `UserProfile` object containing the user's profile information.
-        :rtype: UserProfile
-
-        This method fetches the user profile of the authenticated user. The method calls the `fetch_profile` method of the
-        `account` object to get the profile information. The result is a `UserProfile` object that contains the user's profile
-        information.
-
-        The method returns the `UserProfile` object.
-        """
-        return self.account.fetch_profile()
-
-
-    @authenticated
-    def set_amino_id(self, aminoId: str) -> ApiResponse:
-        """
-        Sets the Amino ID of the authenticated user.
-
-        :param aminoId: The Amino ID to set for the user.
-        :type aminoId: str
-        :return: An `ApiResponse` object containing the server's response to the set Amino ID request.
-        :rtype: ApiResponse
-
-        This method sets the Amino ID of the authenticated user. The Amino ID is passed as a string argument. The method calls
-        the `set_amino_id` method of the `account` object with the `aminoId` parameter set to the given Amino ID. The result
-        is an `ApiResponse` object that contains the server's response to the set Amino ID request.
-
-        The method returns the `ApiResponse` object obtained from calling the `set_amino_id` method of the `account` object.
-        The response will return a `0` status code if the Amino ID is set successfully.
-        """
-        return self.account.set_amino_id(aminoId=aminoId)
-
-
-    @authenticated
-    def fetch_wallet(self) -> Wallet:
-        """
-        Fetches the wallet information for the authenticated user.
-
-        :return: A `Wallet` object containing the user's wallet information.
-        :rtype: Wallet
-
-        This method fetches the wallet information for the authenticated user. The wallet information includes the user's
-        total number of coins, the number of business coins, and other relevant details. The method calls the `fetch_wallet`
-        method of the `account` object. The result is a `Wallet` object that contains the user's wallet information.
-
-        The method returns a `Wallet` object containing the user's wallet information.
+        This method is used to fetch a user's profile.
+        
+        Example usage:
+        
+        >>> x = client.fetch_user("0000-000000-000000-0000-000000")
+        >>> print(x.nickname)
+        "Example"
+        >>> print(x.content)
+        "This is an example profile."
+        >>> print(x.icon)
         """
-        return self.account.fetch_wallet()
-
+        return UserProfile(self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}"
+        ))
+    
 
-    def request_security_validation(self, email: str, resetPassword: bool = False) -> ApiResponse:
+    def edit_profile(
+        self,
+        nickname: str = None,
+        content: str = None,
+        icon: str = None,
+        backgroundColor: str = None,
+        backgroundImage: str = None,
+        defaultBubbleId: str = None
+        ) -> UserProfile:
         """
-        Requests security validation for the provided email address.
-
-        :param email: The email address to request security validation for.
-        :type email: str
-        :param resetPassword: Optional flag to indicate if the user is requesting password reset. Default is False.
-        :type resetPassword: bool
-        :return: An `ApiResponse` object containing the server's response to the security validation request.
-        :rtype: ApiResponse
-
-        This method requests security validation for the provided email address. The email parameter is used to send
-        a validation email to the provided email address. If resetPassword parameter is True, then the email will be sent for
-        password reset. The method calls the `request_security_validation` method of the `account` object with the `email`
-        parameter set to the provided email address and `resetPassword` parameter set to the provided flag. The result is
-        an `ApiResponse` object that contains the server's response to the security validation request.
+        Edits the user's profile.
 
-        The method returns an `ApiResponse` object containing the server's response to the security validation request.
-        """
-        return self.account.request_security_validation(email=email, resetPassword=resetPassword)
+        :param nickname: The new nickname for the user.
+        :type nickname: str
+        :param content: The new content for the user's profile.
+        :type content: str
+        :param icon: The new icon image file for the user.
+        :type icon: str
+        :param backgroundColor: The new background color for the user's profile.
+        :type backgroundColor: str
+        :param backgroundImage: The new background image file for the user's profile.
+        :type backgroundImage: str
+        :param defaultBubbleId: The ID of the default bubble for the user's profile.
+        :type defaultBubbleId: str
+        :return: The response from the account's `edit_profile` method.
+        :rtype: Response
 
+        This method allows the authenticated user to edit their profile settings. Different aspects of the profile can be modified,
+        such as the nickname, content, icon, background color, background image, and default bubble. Only the specified parameters will
+        be updated. The `userId` parameter is set to the authenticated user's ID automatically.
 
-    def activate_email(self, email: str, code: str) -> ApiResponse:
-        """
-        Activates the user's email using the provided verification code.
+        **Example usage:**
 
-        :param email: The email address to activate.
-        :type email: str
-        :param code: The verification code sent to the email address for activation.
-        :type code: str
-        :return: An `ApiResponse` object containing the server's response to the activation request.
-        :rtype: ApiResponse
+        To change the nickname and icon for the user:
 
-        This method activates the user's email using the provided verification code. The email and verification code
-        parameters are used to authenticate the request. The method returns an `ApiResponse` object containing the server's
-        response to the activation request.
+        >>> response = client.edit_profile(nickname="New Nickname", icon="path/to/icon.jpg")
+        ... if response.status == 200:
+        ...     print("Profile edited successfully!")
+        ... else:
+        ...     print("Failed to edit profile.")
         """
-        return self.account.activate_email(email=email, code=code)
-
+        data = {
+                "address": None,
+                "latitude": 0,
+                "longitude": 0,
+                "mediaList": None,
+                "eventSource": "UserProfileView",
+                "timestamp": int(time() * 1000),
+        }
 
-    @authenticated
-    def reset_password(self, email: str, newPassword: str, code: str) -> ResetPassword:
-        """
-        Resets the user's password using the provided email, verification code, and new password.
+        if nickname: data['nickname'] = nickname
+        if icon: data['icon'] = self.upload_image(icon)
+        if content: data['content'] = content
+        if backgroundColor:
+            data["extensions"] = {
+                "style": {
+                    "backgroundColor": backgroundColor
+                    if backgroundColor.startswith("#")
+                    else f"#{backgroundColor}"
+                }
+            }
 
-        :param email: The email address associated with the account.
-        :type email: str
-        :param newPassword: The new password to use for the account.
-        :type newPassword: str
-        :param code: The verification code sent to the email address for account verification.
-        :type code: str
-        :return: A `ResetPassword` object containing the user's session ID and user ID.
-        :rtype: ResetPassword
+        if backgroundImage:
+            data["extensions"] = {
+                "style": {
+                    "backgroundMediaList": [
+                        [100, self.upload_image(backgroundImage), None, None, None]
+                    ]
+                }
+            }
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
-        This method resets the user's password using the provided email, verification code, and new password. The email,
-        verification code, and new password parameters are used to authenticate the request. The method returns a `ResetPassword`
-        object containing the user's session ID and user ID.
-        """
-        return self.account.reset_password(email=email, newPassword=newPassword, code=code)
+        return UserProfile(self.make_request(
+            method = "POST",
+            url = f"/g/s/user-profile/{self.userId}",
+            data = data
+        ))
 
 
     @authenticated
     def send_message(self, content: str, chatId: str, **kwargs) -> CMessage:
         """
         Sends a message to a chat thread.
 
@@ -1150,16 +183,17 @@
         :return: A `CMessage` object containing the details of the sent message.
         :rtype: CMessage
 
         This method sends a message to a chat thread. The content and chat ID parameters are required. Additional parameters
         can be passed as keyword arguments. The method calls the `PrepareMessage` object's `json` method to prepare the message
         data. The result is a `CMessage` object containing the details of the sent message.
         """
-        return CMessage(self.request.handler(
-            method="POST", url=f"/g/s/chat/thread/{chatId}/message",
+        return CMessage(self.make_request(
+            method="POST",
+            url=f"/g/s/chat/thread/{chatId}/message",
             data = PrepareMessage(content=content, **kwargs).json()
             ))
 
 
     @authenticated
     def edit_profile(
         self,
@@ -1198,22 +232,50 @@
 
         >>> response = client.edit_profile(nickname="New Nickname", icon="path/to/icon.jpg")
         ... if response.status == 200:
         ...     print("Profile edited successfully!")
         ... else:
         ...     print("Failed to edit profile.")
         """
-        return self.account.edit_profile(userId = self.userId,
-                                         nickname = nickname,
-                                         content = content,
-                                         icon = icon,
-                                         backgroundColor = backgroundColor,
-                                         backgroundImage = backgroundImage,
-                                         defaultBubbleId = defaultBubbleId
-                                         )
+        data = {
+                "address": None,
+                "latitude": 0,
+                "longitude": 0,
+                "mediaList": None,
+                "eventSource": "UserProfileView",
+                "timestamp": int(time() * 1000),
+        }
+
+        if nickname: data['nickname'] = nickname
+        if icon: data['icon'] = self.upload_image(icon)
+        if content: data['content'] = content
+        if backgroundColor:
+            data["extensions"] = {
+                "style": {
+                    "backgroundColor": backgroundColor
+                    if backgroundColor.startswith("#")
+                    else f"#{backgroundColor}"
+                }
+            }
+
+        if backgroundImage:
+            data["extensions"] = {
+                "style": {
+                    "backgroundMediaList": [
+                        [100, self.upload_image(backgroundImage), None, None, None]
+                    ]
+                }
+            }
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+
+        return UserProfile(self.make_request(
+            method = "POST", url = f"/g/s/user-profile/{self.userId}",
+            data = data
+        ))
 
 
     @authenticated
     def start_chat(
         self,
         userId: Union[str, list],
         message: str,
@@ -1255,33 +317,35 @@
 
         if isGlobal: data.update({"type": 2, "eventSource": "GlobalComposeMenu"})
         else: data["type"] = 0
 
         if publishToGlobal: data["publishToGlobal"] = 1
 
         return ChatThread(
-            self.request.handler(method="POST", url="/g/s/chat/thread", data=data)
+            self.make_request(method="POST", url="/g/s/chat/thread", data=data)
         )
-    
+
+
     @authenticated
-    def blocker_users(self, start: int = 0, size: int = 25):
+    def blocker_users(self, start: int = 0, size: int = 25) -> List[str]:
         """
         Retrieves a list of users what are blocking the logged account.
         :param start: The index to start retrieving the list from (optional, default: 0).
         :type start: int, optional
         :param size: The number of users to retrieve (optional, default: 25).
         :type size: int, optional
         :return: A list of user IDs representing the blocker users.
         :rtype: list
         """
-        return self.request.handler(
+        return self.make_request(
             method = "GET",
             url = f"/g/s/block/full-list?start={start}&size={size}"
         )["blockerUidList"]
 
+
     def fetch_wall_comments(self, userId: str, sorting: str = "newest", start: int = 0, size: int = 25) -> CommentList:
         """
         Fetches wall comments for a user.
 
         :param userId: The ID of the user whose wall comments will be fetched.
         :type userId: str
         :param sorting: The sorting method for the comments. Options: "newest" (default), "oldest", "top".
@@ -1307,21 +371,22 @@
         ...     print(comment.content)
         """
         if sorting.lower() == "newest": sorting = "newest"
         elif sorting.lower() == "oldest": sorting = "oldest"
         elif sorting.lower() == "top": sorting = "vote"
         else: raise ValueError("Incorrect sorting method.")
 
-        return CommentList(self.request.handler(
+        return CommentList(self.make_request(
             method = "GET",
             url = f"/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}"
         ))
-    
+
+
     @authenticated
-    def delete_message(self, chatId: str, messageId: str):
+    def delete_message(self, chatId: str, messageId: str) -> ApiResponse:
         """
         Deletes a message in a chat thread.
 
         :param chatId: The ID of the chat thread where the message is located.
         :type chatId: str
         :param messageId: The ID of the message to delete.
         :type messageId: str
@@ -1340,37 +405,40 @@
 
         >>> response = client.delete_message(chatId="00000000-0000-0000-0000-000000000000", messageId="00000000-0000-0000-0000-000000000000")
         >>> if response.success:
         ...     print("Message deleted successfully!")
         ... else:
         ...     print("Failed to delete message.")
         """
-        return ApiResponse(self.request.handler(
+        return ApiResponse(self.make_request(
             method = "DELETE",
             url = f"/g/s/chat/thread/{chatId}/message/{messageId}"
         ))
-    
+
+
     @authenticated
-    def edit_chat(self,
-                  chatId: str,
-                  doNotDisturb: bool = None,
-                  pinChat: bool = None,
-                  title: str = None,
-                  icon: str = None,
-                  backgroundImage: str = None,
-                  content: str = None,
-                  announcement: str = None,
-                  coHosts: list = None,
-                  keywords: list = None,
-                  pinAnnouncement: bool = None,
-                  publishToGlobal: bool = None,
-                  canTip: bool = None,
-                  viewOnly: bool = None,
-                  canInvite: bool = None,
-                  fansOnly: bool = None) -> list:
+    def edit_chat(
+        self,
+        chatId: str,
+        doNotDisturb: bool = None,
+        pinChat: bool = None,
+        title: str = None,
+        icon: str = None,
+        backgroundImage: str = None,
+        content: str = None,
+        announcement: str = None,
+        coHosts: list = None,
+        keywords: list = None,
+        pinAnnouncement: bool = None,
+        publishToGlobal: bool = None,
+        canTip: bool = None,
+        viewOnly: bool = None,
+        canInvite: bool = None,
+        fansOnly: bool = None
+        ) -> list:
         """
         Edits the settings of a chat.
 
         :param chatId: The ID of the chat to be edited.
         :type chatId: str
         :param doNotDisturb: Set to True to enable "Do Not Disturb" mode for the chat, False to disable it. Default is None.
         :type doNotDisturb: bool, optional
@@ -1433,77 +501,78 @@
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if publishToGlobal: data["publishToGlobal"] = 0
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         responses = []
 
         if doNotDisturb is not None:
-            responses.append(ApiResponse(self.request.handler(
+            responses.append(ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/member/{self.userId}/alert",
                 data = {
                     "alertOption": 2 if doNotDisturb else 1,
                     "timestamp": int(time() * 1000)
                 }
             )).status_code)
         
         if pinChat is not None:
-            responses.append(ApiResponse(self.request.handler(
+            responses.append(ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/{'pin' if pinChat else 'unpin'}"
             )).status_code)
         
         if backgroundImage is not None:
-            responses.append(ApiResponse(self.request.handler(
+            responses.append(ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/member/{self.userId}/background",
                 data = {
                     "media": [100, self.upload_image(backgroundImage), None],
                     "timestamp": int(time() * 1000)
                 }
             )).status_code)
         
         if coHosts is not None:
-            responses.append(ApiResponse(self.request.handler(
+            responses.append(ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/co-host",
                 data = {
                     "uidList": coHosts,
                     "timestamp": int(time() * 1000)
                 }
             )).status_code)
         
         if viewOnly is not None:
-            responses.append(ApiResponse(self.request.handler(
+            responses.append(ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/view-only/{'enable' if viewOnly else 'disable'}"
             )).status_code)
         
         if canInvite is not None:
-            responses.append(ApiResponse(self.request.handler(
+            responses.append(ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/members-can-invite/{'enable' if canInvite else 'disable'}"
             )).status_code)
         
         if canTip is not None:
             responses.append(ApiResponse(
                 method = "POST",
                 url = f"/g/s/chat/thread/{chatId}/tipping-perm-status/{'enable' if canTip else 'disable'}"
             ).status_code)
         
-        responses.append(ApiResponse(self.request.handler(
+        responses.append(ApiResponse(self.make_request(
             method = "POST",
             url = f"/g/s/chat/thread/{chatId}",
             data = data
         )).status_code)
 
         return responses
-    
+
+
     @authenticated
-    def follow(self, userId: Union[str, list]):
+    def follow(self, userId: Union[str, list]) -> ApiResponse:
         """
         Follows a user or a list of users.
 
         :param userId: The ID of the user or a list of user IDs to follow.
         :type userId: Union[str, list]
         :return: The status code of the API response.
         :rtype: int
@@ -1534,20 +603,1239 @@
         >>> response_code = client.follow(userId=user_ids)
         >>> if response_code == 200:
         ...     print("Users followed successfully!")
         ... else:
         ...     print("Failed to follow users.")
         """
         if isinstance(userId, str):
-            return ApiResponse(self.request.handler(
+            return ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/user-profile/{userId}/member"
-            )).status_code
+            ))
         if isinstance(userId, list):
-            return ApiResponse(self.request.handler(
+            return ApiResponse(self.make_request(
                 method = "POST",
                 url = f"/g/s/user-profile/{self.userId}/joined",
                 data = {
                     "targetUidList": userId,
                     "timestamp": int(time() * 1000)
                 }
-            )).status_code
+            ))
+
+
+    @authenticated
+    def fetch_chats(self, start: int = 0, size: int = 25) -> ChatThreadList:
+        """
+        Fetches the chat threads for the authenticated user.
+
+        :param start: The starting index of the chat threads to fetch. (Default: 0)
+        :type start: int, optional
+        :param size: The number of chat threads to fetch. (Default: 25)
+        :type size: int, optional
+        :return: A `ChatThreadList` object containing the fetched chat threads.
+        :rtype: ChatThreadList
+
+        This function sends a GET request to the API to fetch the chat threads that the authenticated user has joined.
+
+        `ChatThreadList` represents a list of chat threads.
+
+        **Example usage:**
+
+        >>> threads = client.fetch_chats(start=0, size=10)
+        ... for thread in threads:
+        ...     print(thread.title)
+        """
+        return ChatThreadList(self.make_request(
+            method = "GET",
+            url = f"/g/s/chat/thread?type=joined-me&start={start}&size={size}"
+        ))
+
+
+    @authenticated
+    def fetch_chat(self, chatId: str) -> ChatThread:
+        """
+        Fetches a chat thread by its ID.
+
+        :param chatId: The ID of the chat thread to fetch.
+        :type chatId: str
+        :return: A `ChatThread` object representing the fetched chat thread.
+        :rtype: ChatThread
+
+        This function sends a GET request to the API to fetch a chat thread based on its ID.
+
+        `ChatThread` represents a thread of messages in a chat.
+
+        **Example usage:**
+
+        >>> chat = client.fetch_chat("123456789")
+        ... print(chat.thread_id)
+        ... print(chat.messages)
+        """
+        return ChatThread(self.make_request(
+            method = "GET",
+            url = f"/g/s/chat/thread/{chatId}"
+        ))
+
+
+    @authenticated
+    def fetch_chat_users(self, chatId: str, start: int = 0, size: int = 25) -> CChatMembers:
+        """
+        Fetches the users in a chat.
+
+        :param chatId: The ID of the chat.
+        :type chatId: str
+        :param start: The start index for fetching the users. (Default: 0)
+        :type start: int, optional
+        :param size: The number of users to fetch. (Default: 25)
+        :type size: int, optional
+        :return: A `CChatMembers` object containing the chat members.
+        :rtype: CChatMembers
+
+        This function retrieves the users who are members of the specified chat.
+
+        `CChatMembers` represents the members of a chat.
+
+        **Example usage:**
+
+        >>> chat_members = client.fetch_chat_users("chat123")
+        ... for member in chat_members.nickname:
+        ...     print(member)
+        """
+        return CChatMembers(self.make_request(
+            method = "GET",
+            url = f"/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2"
+        ))
+
+
+    @authenticated
+    def invite_to_chat(self, chatId: str, userId: Union[str, list]) -> ApiResponse:
+        """
+        Invites user(s) to a chat.
+
+        :param chatId: The ID of the chat to invite users to.
+        :type chatId: str
+        :param userId: The ID(s) of the user(s) to invite. It can be a string or a list of strings.
+        :type userId: Union[str, list]
+        :return: An `ApiResponse` object representing the response of the invitation request.
+        :rtype: ApiResponse
+        :raises TypeError: If userId is neither a string nor a list of strings.
+
+        This function sends a POST request to invite user(s) to a chat.
+
+        The user(s) specified by userId will be invited to join the chat identified by chatId.
+
+        `ApiResponse` represents the response of an API request.
+
+        **Example usage:**
+
+        >>> response = client.invite_to_chat("chat123", "user456")
+        ... print(response.status_code)
+        """
+        if isinstance(userId, str): userIds = [userId]
+        elif isinstance(userId, list): userIds = userId
+        else: raise TypeError("UserId must be a string or a list of strings.")
+
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/g/s/chat/thread/{chatId}/member/invite",
+            data = {
+                "timestamp": int(time() * 1000),
+                "uids": userIds
+            }
+        ))
+
+
+    @authenticated
+    def kick(self, chatId: str, userId: str, allowRejoin: bool = True) -> ApiResponse:
+        """
+        Kicks a user from a chat.
+
+        :param chatId: The ID of the chat.
+        :type chatId: str
+        :param userId: The ID of the user to be kicked.
+        :type userId: str
+        :param allowRejoin: Whether to allow the user to rejoin the chat. (Default: True)
+        :type allowRejoin: bool, optional
+        :return: An `ApiResponse` object representing the API response.
+        :rtype: ApiResponse
+
+        This function sends a DELETE request to the API to kick the specified user from the chat.
+
+        `ApiResponse` represents the response from the API.
+
+        **Example usage:**
+
+        >>> response = client.kick("chat123", "user456")
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(self.make_request(
+            method = "DELETE",
+            url = f"/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}"
+        ))
+
+
+    @authenticated
+    def fetch_messages(self, chatId: str, size: int = 25, pageToken: str = None) -> CMessages:
+        """
+        Fetches messages from a chat.
+
+        :param chatId: The ID of the chat to fetch messages from.
+        :type chatId: str
+        :param size: The number of messages to fetch. (Default: 25)
+        :type size: int, optional
+        :param pageToken: The page token for pagination. (Optional)
+        :type pageToken: str, optional
+        :return: A `CMessages` object representing the fetched messages.
+        :rtype: CMessages
+
+        This function retrieves messages from the specified chat using the provided parameters.
+
+        `CMessages` represents a collection of messages in the chat.
+
+        **Example usage:**
+
+        >>> messages = client.fetch_messages("chat123", size=50, pageToken="token123")
+        ... for message in messages:
+        ...     print(message.text)
+        """
+        if pageToken is not None:
+            return CMessages(self.make_request(
+                method = "GET",
+                url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
+            ))
+        return CMessages(self.make_request(
+            method = "GET",
+            url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
+        ))
+
+
+    @authenticated
+    def fetch_message(self, chatId: str, messageId: str) -> Message:
+        """
+        Fetches a specific message from a chat thread.
+
+        :param chatId: The ID of the chat thread.
+        :type chatId: str
+        :param messageId: The ID of the message to fetch.
+        :type messageId: str
+        :return: A `Message` object representing the fetched message.
+        :rtype: Message
+
+        This function retrieves a specific message with the given `messageId` from the chat thread specified by `chatId`.
+
+        `Message` represents a message in a chat thread.
+
+        **Example usage:**
+
+        >>> message = client.fetch_message("chat123", "message456")
+        ... print(message.text)
+        ... print(message.timestamp)
+        """
+        return Message(self.make_request(
+            method = "GET",
+            url = f"/g/s/chat/thread/{chatId}/message/{messageId}"
+        ))
+
+
+    @authenticated
+    def search_community(self, aminoId: str) -> dict:
+        """
+        Search for a community by Amino ID or link.
+
+        :param aminoId: The Amino ID or link of the community to search for.
+        :type aminoId: str
+        :return: A dictionary containing the search results.
+        :rtype: dict
+
+        This function sends a GET request to search for a community using the specified Amino ID or link.
+
+        **Example usage:**
+
+        >>> search_results = client.search_community("example_community").title
+        ... print(search_results)
+        """
+        return self.make_request(
+            method = "GET",
+            url = f"/g/s/search/amino-id-and-link?q={aminoId}"
+        )
+
+
+    @authenticated
+    def fetch_followers(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
+        """
+        Fetches the followers of a user.
+
+        :param userId: The ID of the user to fetch the followers for.
+        :type userId: str
+        :param start: The starting index of the followers list. (Default: 0)
+        :type start: int, optional
+        :param size: The number of followers to fetch. (Default: 25)
+        :type size: int, optional
+        :return: A `UserProfileList` object containing the fetched followers.
+        :rtype: UserProfileList
+
+        This function sends a GET request to the API to fetch the followers of a user.
+
+        `UserProfileList` represents a list of user profiles.
+
+        **Example usage:**
+
+        >>> followers = client.fetch_followers("user123", start=0, size=10)
+        ... for follower in followers.userId:
+        ...     print(follower)
+        """
+        return UserProfileList(self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/member?start={start}&size={size}"
+        ))
+
+
+    @authenticated
+    def fetch_following(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
+        """
+        Fetches the user profiles of the users that the specified user is following.
+
+        :param userId: The ID of the user.
+        :type userId: str
+        :param start: The index to start fetching from. (Default: 0)
+        :type start: int, optional
+        :param size: The number of user profiles to fetch. (Default: 25)
+        :type size: int, optional
+        :return: A `UserProfileList` object containing the user profiles.
+        :rtype: UserProfileList
+
+        This function sends a GET request to the API to fetch the user profiles of the users that the specified user is following.
+
+        `UserProfileList` represents a list of user profiles.
+
+        **Example usage:**
+
+        >>> following = client.fetch_following("user123")
+        ... for profile in following.userId:
+        ...     print(profile)
+        """
+        return UserProfileList(self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/joined?start={start}&size={size}"
+        ))
+
+
+    @authenticated
+    def fetch_visitors(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
+        """
+        Fetches the visitors of a user profile.
+
+        :param userId: The ID of the user profile to fetch visitors for.
+        :type userId: str
+        :param start: The index of the first visitor to retrieve. (Default: 0)
+        :type start: int, optional
+        :param size: The maximum number of visitors to retrieve. (Default: 25)
+        :type size: int, optional
+        :return: A `UserProfileList` object containing the retrieved user profiles.
+        :rtype: UserProfileList
+
+        This function sends a GET request to the API to fetch the visitors of a user profile.
+
+        `UserProfileList` represents a list of user profiles.
+
+        **Example usage:**
+
+        >>> visitors = client.fetch_visitors("123456", start=0, size=10)
+        ... for visitor in visitors.userId:
+        ...     print(visitor)
+        """
+        return UserProfileList(self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/visitors?start={start}&size={size}"
+        ))
+
+
+    @authenticated
+    def blocked_users(self, start: int = 0, size: int = 25):
+        """
+        Retrieves a list of blocked users.
+
+        :param start: The index of the first blocked user to retrieve. (Default: 0)
+        :type start: int, optional
+        :param size: The maximum number of blocked users to retrieve. (Default: 25)
+        :type size: int, optional
+        :return: A `UserProfileList` object containing the list of blocked users.
+        :rtype: UserProfileList
+
+        This function sends a GET request to the API to retrieve a list of blocked users.
+
+        `UserProfileList` represents a list of user profiles.
+
+        **Example usage:**
+
+        >>> blocked_users = client.blocked_users(start=0, size=10)
+        ... for user in blocked_users.userId:
+        ...     print(user)
+        """
+        return UserProfileList(self.make_request(
+            method = "GET",
+            url = f"/g/s/block?start={start}&size={size}"
+        ))
+
+
+    @authenticated
+    def mark_as_read(self, chatId: str, messageId: str) -> ApiResponse:
+        """
+        Marks a message as read.
+        
+        :param chatId: The ID of the chat to mark the message as read in.
+        :type chatId: str
+        :param messageId: The ID of the message to mark as read.
+        :type messageId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to mark a message as read.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.mark_as_read("000000-0000-0000-000000", "000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/g/s/chat/thread/{chatId}/mark-as-read",
+            data = {
+                "messageId": messageId,
+                "timestamp": int(time() * 1000)
+            }
+        ))
+
+
+    @authenticated
+    def visit(self, userId: str) -> ApiResponse:
+        """
+        Visits a user profile.
+        
+        :param userId: The ID of the user profile to visit.
+        :type userId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to visit a user profile.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.visit("000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/g/s/user-profile/{userId}?action=visit"
+        ))
+
+
+    @authenticated
+    def block(self, userId: str) -> ApiResponse:
+        """
+        Blocks a user.
+        
+        :param userId: The ID of the user to block.
+        :type userId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to block a user.
+
+        `ApiResponse` represents a response from the API.
+
+        **Example usage:**
+
+        >>> x = client.block("000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/g/s/block/{userId}"
+        ))
+
+
+    @authenticated
+    def unblock(self, userId: str) -> ApiResponse:
+        """
+        Unblocks a user.
+        
+        :param userId: The ID of the user to unblock.
+        :type userId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to unblock a user.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.unblock("000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "DELETE",
+            url = f"/g/s/block/{userId}"
+        ))
+
+
+    @authenticated
+    def join_request(self, comId: str, message: str = None):
+        """
+        Sends a join request to a community.
+        
+        :param comId: The ID of the community to send the join request to.
+        :type comId: str
+        :param message: The message to send with the join request.
+        :type message: str, optional
+        
+        This function sends a POST request to the API to send a join request to a community.
+
+        `ApiResponse` represents a response from the API.
+
+        **Example usage:**
+
+        >>> x = client.join_request("000000-0000-0000-000000", "Hello! I would like to join this community.")
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/x{comId}/s/community/membership-request",
+            data = {
+                "message": message,
+                "timestamp": int(time() * 1000)
+            }
+        ))
+
+
+    @authenticated
+    def flag_community(
+        self,
+        comId: str,
+        reason: str,
+        flagType: FlagTypes = FlagTypes.OFFTOPIC,
+        isGuest: bool = False
+        ) -> ApiResponse:
+        """
+        Flags a community.
+        
+        :param comId: The ID of the community to flag.
+        :type comId: str
+        :param reason: The reason for flagging the community.
+        :type reason: str
+        :param flagType: The type of flag to send.
+        :type flagType: FlagTypes, optional
+        :param isGuest: Whether or not the flag is from a guest account.
+        :type isGuest: bool, optional
+        
+        This function sends a POST request to the API to flag a community.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.flag_community("000000-0000-0000-000000", "This community is offensive.", 1)
+        ... print(x.status_code)
+        """
+        if reason is None: raise ValueError("Reason must be specified.")
+        if flagType is None: raise ValueError("Flag type must be specified.")
+
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/x{comId}/s/item-flag",
+            data = {
+                "flagType": flagType.value if isinstance(flagType, FlagTypes) else flagType,
+                "reason": reason,
+                "timestamp": int(time() * 1000),
+                "isGuest": "g-flag" if isGuest else "flag"
+            }
+        ))
+
+
+    def fetch_linked_communities(self, userId: str) -> list:
+        """
+        Fetches a user's linked communities.
+        
+        :param userId: The ID of the user to fetch the linked communities of.
+        :type userId: str
+        :return: A list of linked communities.
+        :rtype: list
+        
+        This function sends a GET request to the API to fetch a user's linked communities.
+        
+        **Example usage:**
+        
+        >>> x = client.fetch_linked_communities("000000-0000-0000-000000")
+        ... print(x)
+        """
+        return self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/linked-community"
+        )["linkedCommunityList"]
+
+
+    def fetch_unlinked_communities(self, userId: str) -> list:
+        """
+        Fetches a user's unlinked communities.
+        
+        :param userId: The ID of the user to fetch the unlinked communities of.
+        :type userId: str
+        :return: A list of unlinked communities.
+        :rtype: list
+        
+        This function sends a GET request to the API to fetch a user's unlinked communities.
+        
+        **Example usage:**
+        
+        >>> x = client.fetch_unlinked_communities("000000-0000-0000-000000")
+        ... print(x)
+        """
+        return self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/unlinked-community"
+        )["unlinkedCommunityList"]
+
+
+    @authenticated
+    def reorder_linked_communities(self, comIds: List[int]) -> ApiResponse:
+        """
+        Reorders a user's linked communities.
+        
+        :param comIds: A list of community IDs to reorder.
+        :type comIds: List[int]
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to reorder a user's linked communities.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.reorder_linked_communities([3, 2, 1])
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/g/s/user-profile/{self.userId}/linked-community/reorder",
+            data = {
+                "timestamp": int(time() * 1000),
+                "comIds": comIds
+            }
+        ))
+
+
+    @authenticated
+    def add_linked_community(self, comId: int) -> ApiResponse:
+        """
+        Adds a linked community to a user's profile.
+        
+        :param comId: The ID of the community to add.
+        :type comId: int
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to add a linked community to a user's profile.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.add_linked_community(3)
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "POST",
+            url = f"/g/s/user-profile/{self.userId}/linked-community/{comId}"
+        ))
+
+
+    @authenticated
+    def remove_linked_community(self, comId: int) -> ApiResponse:
+        """
+        Removes a linked community from a user's profile.
+        
+        :param comId: The ID of the community to remove.
+        :type comId: int
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to remove a linked community from a user's profile.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.remove_linked_community(1)
+        ... print(x.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "DELETE",
+            url = f"/g/s/user-profile/{self.userId}/linked-community/{comId}"
+        ))
+
+
+    @authenticated
+    def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None) -> ApiResponse:
+        """
+        Comments on a user's profile, blog, or wiki.
+        
+        :param message: The message to comment.
+        :type message: str
+        :param userId: The ID of the user to comment on.
+        :type userId: str
+        :param blogId: The ID of the blog to comment on.
+        :type blogId: str
+        :param wikiId: The ID of the wiki to comment on.
+        :type wikiId: str
+        :param replyTo: The ID of the comment to reply to.
+        :type replyTo: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to comment on a user's profile, blog, or wiki.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.comment("Hello, world!", userId = "000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        if message is None: raise ValueError("Message must be specified.")
+
+        data = {
+            "content": message,
+            "stickerId": None,
+            "type": 0,
+            "timestamp": int(time() * 1000)
+        }
+
+        if replyTo: data["respondTo"] = replyTo
+
+        if userId:
+            data["eventSource"] = "UserProfileView"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/user-profile/{userId}/g-comment",
+                data = data
+            ))
+
+        elif blogId:
+            data["eventSource"] = "PostDetailView"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/blog/{blogId}/g-comment",
+                data = data
+            ))
+        
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            url = f"/g/s/item/{wikiId}/g-comment"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/item/{wikiId}/g-comment"
+            ))
+        
+        else:
+            raise ValueError("Either userId, blogId or wikiId must be specified.")
+
+
+    @authenticated
+    def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> ApiResponse:
+        """
+        Deletes a comment on a user's profile, blog, or wiki.
+        
+        :param commentId: The ID of the comment to delete.
+        :type commentId: str
+        :param userId: The ID of the user to delete the comment from.
+        :type userId: str
+        :param blogId: The ID of the blog to delete the comment from.
+        :type blogId: str
+        :param wikiId: The ID of the wiki to delete the comment from.
+        :type wikiId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to delete a comment on a user's profile, blog, or wiki."""
+        if userId:
+            return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/user-profile/{userId}/g-comment/{commentId}"
+            ))
+        elif blogId:
+            return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/blog/{blogId}/g-comment/{commentId}"
+            ))
+        elif wikiId:
+            return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/item/{wikiId}/g-comment/{commentId}"
+            ))
+        else:
+            raise ValueError("Either userId, blogId or wikiId must be specified.")
+
+
+    @authenticated
+    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None) -> ApiResponse:
+        """
+        Likes a blog or wiki.
+        
+        :param blogId: The ID of the blog to like.
+        :type blogId: Union[str, list]
+        :param wikiId: The ID of the wiki to like.
+        :type wikiId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a POST request to the API to like a blog or wiki.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.like_blog("000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        data = {"value": 4, "timestamp": int(time() * 1000)}
+
+        if blogId:
+            if isinstance(blogId, str):
+                data["eventSource"] = "UserProfileView",
+                return ApiResponse(self.make_request(
+                    method = "POST",
+                    url = f"/g/s/blog/{blogId}/g-vote?cv=1.2",
+                    data = data
+                ))
+            elif isinstance(blogId, list):
+                data["targetIdList"] = blogId,
+                return ApiResponse(
+                    self.make_request(
+                        method = "POST", url="/g/s/feed/g-vote",
+                        data = data
+                    )
+                )
+            else: raise TypeError("blogId must be a string or a list.")
+
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/item/{wikiId}/g-vote?cv=1.2",
+                data = data
+            ))
+        else:
+            raise ValueError("Either blogId or wikiId must be specified.")
+
+
+    @authenticated
+    def unlike_blog(self, blogId: str = None, wikiId: str = None) -> ApiResponse:
+        """
+        Unlikes a blog or wiki.
+        
+        :param blogId: The ID of the blog to unlike.
+        :type blogId: str
+        :param wikiId: The ID of the wiki to unlike.
+        :type wikiId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to unlike a blog or wiki.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.unlike_blog("000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        
+        if blogId: return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"{self.api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView"
+            ))
+        elif wikiId: return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView"
+            ))
+        else:
+            raise ValueError("Either blogId or wikiId must be specified.")
+
+
+    @authenticated
+    def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> ApiResponse:
+        """
+        Likes a comment on a user's profile, blog, or wiki.
+        
+        :param commentId: The ID of the comment to like.
+        :type commentId: str
+        :param userId: The ID of the user to like the comment on.
+        :type userId: str
+        :param blogId: The ID of the blog to like the comment on.
+        :type blogId: str
+        :param wikiId: The ID of the wiki to like the comment on.
+        :type wikiId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to like a comment on a user's profile, blog, or wiki.
+
+        `ApiResponse` represents a response from the API.
+
+        **Example usage:**
+
+        >>> x = client.like_comment("000000-0000-0000-000000", userId="000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        data = {"value": 4, "timestamp": int(time() * 1000)}
+
+        if userId:
+            data["eventSource"] = "UserProfileView"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1",
+                data = data
+                ))
+        
+        elif blogId:
+            data["eventSource"] = "PostDetailView"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/blog/{blogId}/comment/{commentId}/g-vote?cv=1.2&value=1",
+                data = data
+            ))
+        
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            return ApiResponse(self.make_request(
+                method = "POST",
+                url = f"/g/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1",
+                data = data
+            ))
+        
+        else: raise ValueError("Either userId, blogId or wikiId must be specified.")
+
+
+    @authenticated
+    def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> ApiResponse:
+        """
+        Unlikes a comment on a user's profile, blog, or wiki.
+        
+        :param commentId: The ID of the comment to unlike.
+        :type commentId: str
+        :param userId: The ID of the user to unlike the comment on.
+        :type userId: str
+        :param blogId: The ID of the blog to unlike the comment on.
+        :type blogId: str
+        :param wikiId: The ID of the wiki to unlike the comment on.
+        :type wikiId: str
+        :return: An `ApiResponse` object containing the response from the API.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to unlike a comment on a user's profile, blog, or wiki.
+        
+        `ApiResponse` represents a response from the API.
+        
+        **Example usage:**
+        
+        >>> x = client.unlike_comment("000000-0000-0000-000000", userId="000000-0000-0000-000000")
+        ... print(x.status_code)
+        """
+        if userId:
+            return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView"
+            ))
+        elif blogId:
+            return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
+            ))
+        elif wikiId:
+            return ApiResponse(self.make_request(
+                method = "DELETE",
+                url = f"/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
+            ))
+        else: raise ValueError("Either userId, blogId or wikiId must be specified.")
+
+
+    def fetch_supported_languages(self) -> List[str]:
+        """
+        Fetches a list of supported languages for the API.
+        
+        :return: A list of supported languages.
+        :rtype: List[str]
+        
+        This function sends a GET request to the API to fetch a list of supported languages.
+        
+        **Example usage:**
+        
+        >>> x = client.fetch_supported_languages()
+        ... print(x)
+        """
+        return self.make_request(
+            method="GET",
+            url="/g/s/community-collection/supported-languages?start=0&size=100",
+        )["supportedLanguages"]
+
+
+    @authenticated
+    def fetch_ta_announcement(self, language: str = "en", start: int = 0, size: int = 25) -> dict:
+        """
+        Fetches the latest announcements from the API.
+
+        :param language: The language to fetch the announcements in.
+        :type language: str
+        :param start: The index to start fetching announcements from.
+        :type start: int
+        :param size: The number of announcements to fetch.
+        :type size: int
+        :return: A dictionary containing the announcements.
+        :rtype: dict
+
+        This function sends a GET request to the API to fetch the latest announcements.
+
+        **Example usage:**
+
+        >>> x = client.fetch_ta_announcement()
+        ... print(x)
+        """
+        if language not in self.fetch_supported_languages():
+            raise ValueError("Invalid language.")
+        
+        return self.make_request(
+            method = "GET",
+            url = f"/g/s/announcement?language={language}&start={start}&size={size}"
+        )
+
+
+    @authenticated
+    def join_chat(self, chatId: str) -> ApiResponse:
+        """
+        Joins the authenticated user to a chat thread.
+
+        :param chatId: The ID of the chat thread to join.
+        :type chatId: str
+        :return: The API response.
+        :rtype: ApiResponse
+
+        This method joins the authenticated user to a chat thread. The user must be a member of the community that the chat
+        thread belongs to in order to join the thread.
+
+        **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
+        be raised.
+        """
+        return ApiResponse(self.make_request(
+            method="POST",
+            url=f"/g/s/chat/thread/{chatId}/member/{self.userId}"
+            ))
+
+
+    @authenticated
+    def leave_chat(self, chatId: str) -> ApiResponse:
+        """
+        Removes the authenticated user from a chat thread.
+
+        :param chatId: The ID of the chat thread to leave.
+        :type chatId: str
+        :return: The API response.
+        :rtype: ApiResponse
+
+        This method removes the authenticated user from a chat thread. The user must be a member of the chat thread in order
+        to leave it.
+
+        **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
+        be raised.
+        """
+        return ApiResponse(self.make_request(
+            method="DELETE",
+            url=f"/g/s/chat/thread/{chatId}/member/{self.userId}"
+            ))
+
+
+    @authenticated
+    def join_community(self, community_id: int, invitationId = None) -> ApiResponse:
+        """
+        Joins the user to a community with the provided community ID.
+
+        :param community_id: The ID of the community to join.
+        :type community_id: int
+        :param invitationId: The ID of the invitation link.
+        :type invitationId: str
+        :return: An ApiResponse object containing the server response.
+        :rtype: ApiResponse
+        :raises LoginRequired: If the user is not logged in.
+
+        This function first checks if the client is logged in by checking for a valid session ID. If not, it raises a
+        LoginRequired exception.
+
+        If the client is logged in, the function sends a POST request to the server to join the specified community.
+        The request includes the client's session ID and the ID of the community to join.
+
+        The function returns an ApiResponse object containing the server response.
+
+        **Note:** This function can be used to join the user to a community with the provided community ID. Once joined,
+        the user can make API calls related to the community, such as posting or retrieving posts.
+        """
+        data = {"timestamp": int(time() * 1000)}
+        if invitationId:
+            data["invitationId"] = invitationId
+
+        return ApiResponse(
+            self.make_request(
+                method="POST",
+                url=f"/x{community_id}/s/community/join",
+                data = data
+        ))
+
+
+    @authenticated
+    def leave_community(self, community_id: int) -> ApiResponse:
+        """
+        Leaves the user from a community with the provided community ID.
+
+        :param community_id: The ID of the community to leave.
+        :type community_id: int
+        :return: An ApiResponse object containing the server response.
+        :rtype: ApiResponse
+        :raises LoginRequired: If the user is not logged in.
+
+        This function first checks if the client is logged in by checking for a valid session ID. If not, it raises a
+        LoginRequired exception.
+
+        If the client is logged in, the function sends a POST request to the server to leave the specified community.
+        The request includes the client's session ID and the ID of the community to leave.
+
+        The function returns an ApiResponse object containing the server response.
+
+        **Note:** This function can be used to leave the user from a community with the provided community ID. Once left,
+        the user will no longer have access to the community and will not be able to make API calls related to the community.
+        """
+        return ApiResponse(self.make_request(
+            method="POST",
+            url=f"/x{community_id}/s/community/leave"
+            ))
+    
+
+    def fetch_community(self, community_id: int) -> CCommunity:
+        """
+        Fetches the community information for the community with the provided community ID.
+
+        :param community_id: The ID of the community to fetch.
+        :type community_id: int
+        :return: A CCommunity object representing the community information.
+        :rtype: CCommunity
+
+        This function sends a GET request to the server to fetch the community information for the community with the
+        provided community ID. The request includes the ID of the community to fetch.
+
+        The function returns a CCommunity object representing the community information. The CCommunity object contains
+        attributes such as the members count, the community's layout, and other community information.
+
+        **Note:** This function can be used to fetch the community information for a community on Amino. The community
+        information can be used to display information about the community such as the community's name, description, and
+        other information.
+        """
+        return CCommunity(self.make_request(
+            method="GET",
+            url=f"/g/s-x{community_id}/community/info"
+            ))
+    
+
+    @authenticated
+    def joined_communities(self) -> CCommunityList:
+        """
+        Retrieves the list of communities that the authenticated user has joined.
+
+        :return: The list of communities.
+        :rtype: CCommunityList
+
+        This method returns the list of communities that the authenticated user has joined. The list includes information
+        such as the community ID, name, description, and theme.
+
+        **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
+        be raised.
+        """
+        return CCommunityList(self.make_request(
+            method="GET",
+            url="/g/s/community/joined"
+            ))
+
+
+    def fetch_object_id(self, link: str) -> str:
+        """
+        Fetches the object ID given a link to the object.
+
+        :param link: The link to the object.
+        :type link: str
+        :raises NotLoggedIn: If the user is not logged in.
+        :raises MissingCommunityId: If the community ID is missing.
+        :return: The ID of the object.
+        :rtype: str
+
+        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
+        The method caches the object ID for faster access in future calls.
+
+        **Example usage:**
+
+        >>> object_id = client.community.fetch_object_id(link="https://aminoapps.com/p/w2Fs6H")
+        >>> print(object_id)
+        """
+
+        KEY = str((link, "OBJECT_ID"))
+        if not self.cache.get(KEY):
+            self.cache.set(KEY, self.make_request(
+                method = "GET",
+                url = f"/g/s/link-resolution?q={link}"
+                ))
+        return LinkInfo(self.cache.get(KEY)).objectId
+
+
+    def fetch_object_info(self, link: str) -> LinkInfo:
+        """
+        Fetches information about an object given its link.
+
+        :param link: The link to the object.
+        :type link: str
+        :raises NotLoggedIn: If the user is not logged in.
+        :raises MissingCommunityId: If the community ID is missing.
+        :return: A LinkInfo object containing information about the object.
+        :rtype: LinkInfo
+
+        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
+        The method caches the object information for faster access in future calls.
+
+        `LinkInfo`:
+
+        - `data`: The raw response data from the API.
+        - `linkInfoV2`: The link information data.
+        - `path`: The path of the object.
+        - `extensions`: The extensions data.
+        - `objectId`: The ID of the object.
+        - `shareURLShortCode`: The short code of the share URL.
+        - `targetCode`: The target code.
+        - `ndcId`: The NDC ID.
+        - `comId`: The community ID.
+        - `fullPath`: The full path of the object.
+        - `shortCode`: The short code of the object.
+        - `objectType`: The type of the object.
+
+        **Example usage:**
+
+        >>> object_info = client.community.fetch_object_info(link="https://aminoapps.com/p/w2Fs6H")
+        >>> print(object_info.objectId)
+        """
+
+        KEY = str((link, "OBJECT_INFO"))
+        if not self.cache.get(KEY):
+            self.cache.set(KEY, self.make_request(
+                method = "GET",
+                url = f"/g/s/link-resolution?q={link}"
+                ))
+        return LinkInfo(self.cache.get(KEY))
```

### Comparing `pymino-1.2.1.9/pymino/ext/account.py` & `pymino-1.2.2.1/pymino/ext/account.py`

 * *Files 12% similar despite different names*

```diff
@@ -370,81 +370,8 @@
                     "type": 1,
                     "identity": email,
                     "level": 2,
                     "deviceID": deviceId
                 },
                 "phoneNumberValidationContext": None,
                 "deviceID": deviceId
-            }))
-
-
-    def edit_profile(
-        self,
-        userId: str,
-        nickname: str = None,
-        content: str = None,
-        icon: str = None,
-        backgroundColor: str = None,
-        backgroundImage: str = None,
-        defaultBubbleId: str = None
-        ) -> UserProfile:
-        """
-        `edit_profile` - Edits the user profile.
-
-        `Parameters`:
-        - `userId` (str): The ID of the user profile to edit.
-        - `nickname` (str, optional): The new nickname for the user.
-        - `content` (str, optional): The new content for the user profile.
-        - `icon` (str, optional): The path or URL of the new icon image for the user profile.
-        - `backgroundColor` (str, optional): The new background color for the user profile.
-        - `backgroundImage` (str, optional): The path or URL of the new background image for the user profile.
-        - `defaultBubbleId` (str, optional): The ID of the default bubble for the user profile.
-
-        `Returns`:
-        An instance of the `UserProfile` class representing the updated user profile.
-
-        `Example`:
-        ```python
-        from pymino import *
-
-        bot = Bot()
-        bot.run(email=email, password=password)
-        response = bot.edit_profile(userId="12345", nickname="NewNickname", content="NewContent", backgroundColor="#FFFFFF")
-        print(response.json)
-        ```
-        """
-        data = {
-                "address": None,
-                "latitude": 0,
-                "longitude": 0,
-                "mediaList": None,
-                "eventSource": "UserProfileView",
-                "timestamp": int(time() * 1000),
-        }
-
-        if nickname: data['nickname'] = nickname
-        if icon: data['icon'] = self.upload_image(icon)
-        if content: data['content'] = content
-        if backgroundColor:
-            data["extensions"] = {
-                "style": {
-                    "backgroundColor": backgroundColor
-                    if backgroundColor.startswith("#")
-                    else f"#{backgroundColor}"
-                }
-            }
-
-        if backgroundImage:
-            data["extensions"] = {
-                "style": {
-                    "backgroundMediaList": [
-                        [100, self.upload_image(backgroundImage), None, None, None]
-                    ]
-                }
-            }
-        if defaultBubbleId:
-            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
-
-        return UserProfile(self.session.handler(
-            method = "POST", url = f"/g/s/user-profile/{userId}",
-            data = data
-        ))
+            }))
```

### Comparing `pymino-1.2.1.9/pymino/ext/async_community.py` & `pymino-1.2.2.1/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/async_context.py` & `pymino-1.2.2.1/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/async_event_handler.py` & `pymino-1.2.2.1/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/async_socket.py` & `pymino-1.2.2.1/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/community.py` & `pymino-1.2.2.1/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/console.py` & `pymino-1.2.2.1/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/context.py` & `pymino-1.2.2.1/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/dispatcher.py` & `pymino-1.2.2.1/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/acm.py` & `pymino-1.2.2.1/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/admin_log.py` & `pymino-1.2.2.1/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/api_response.py` & `pymino-1.2.2.1/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/bubble.py` & `pymino-1.2.2.1/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/chat_threads.py` & `pymino-1.2.2.1/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/comments.py` & `pymino-1.2.2.1/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/enums.py` & `pymino-1.2.2.1/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/exceptions.py` & `pymino-1.2.2.1/pymino/ext/entities/exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -492,8 +492,8 @@
             "Ping failed. Please make sure you are logged in and try again."
             )
         
 class IntentsNotEnabled(Exception):
     def __init__(self):
         super().__init__(
             "Intents are not enabled. Please enable them in your Bot instance and try again."
-            )
+            )
```

### Comparing `pymino-1.2.1.9/pymino/ext/entities/general.py` & `pymino-1.2.2.1/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/handlers.py` & `pymino-1.2.2.1/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/link_info.py` & `pymino-1.2.2.1/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/member.py` & `pymino-1.2.2.1/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/messages.py` & `pymino-1.2.2.1/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/notification.py` & `pymino-1.2.2.1/pymino/ext/entities/notification.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def alert(self) -> str:
         """Returns the alert of the notification."""
         return self.aps.get("alert")
     
     @property
     def notification_type(self) -> int:
         """Returns the notification type of the notification."""
-        return self.payload.get("notification_type")
+        return self.payload.get("notifType")
     
     @property
     def id(self) -> str:
         """Returns the ID of the notification."""
         return self.payload.get("id")
     
     def json(self) -> dict:
```

### Comparing `pymino-1.2.1.9/pymino/ext/entities/sticker.py` & `pymino-1.2.2.1/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/threads.py` & `pymino-1.2.2.1/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/userprofile.py` & `pymino-1.2.2.1/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/entities/wsevents.py` & `pymino-1.2.2.1/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/handle_queue.py` & `pymino-1.2.2.1/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/socket.py` & `pymino-1.2.2.1/pymino/ext/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         )
 
 
 try:
     from websocket import WebSocket, WebSocketApp
 except ImportError as e:
     system("pip uninstall websocket -y")
-    system("pip install websocket-client==1.5.2")
+    system("pip install websocket-client==1.6.1")
     raise WrongWebSocketPackage from e
 
 
 class WSClient(EventHandler):
     """
     `WSClient` is a class that handles the websocket.
     """
```

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.2.1/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/chat_console.py` & `pymino-1.2.2.1/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/commands.py` & `pymino-1.2.2.1/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/community_console.py` & `pymino-1.2.2.1/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/generate.py` & `pymino-1.2.2.1/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/menu.py` & `pymino-1.2.2.1/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/profile_console.py` & `pymino-1.2.2.1/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.9/pymino/ext/utilities/request_handler.py` & `pymino-1.2.2.1/pymino/ext/utilities/request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         
         `**Returns**``
         - `Union[int, str]` - The status code and response from the request.
         
         """
         try:
             response: HttpResponse = self.fetch_request(method)(
-                url, data=data, headers=headers, proxies=self.proxy, timeout=10 if self.proxy else 2
+                url, data=data, headers=headers, proxies=self.proxy
             )
             return response.status_code, response.text
         except (
             ConnectionError,
             ReadTimeout,
             SSLError,
             ProxyError,
```

### Comparing `pymino-1.2.1.9/pymino.egg-info/PKG-INFO` & `pymino-1.2.2.1/pymino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.9
+Version: 1.2.2.1
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.9 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.2.1 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.9/pymino.egg-info/SOURCES.txt` & `pymino-1.2.2.1/pymino.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
-pymino/ext/_global.py
 pymino/ext/account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
 pymino/ext/async_socket.py
 pymino/ext/community.py
 pymino/ext/console.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
+pymino/ext/global_client.py
 pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
 pymino/ext/entities/acm.py
 pymino/ext/entities/admin_log.py
 pymino/ext/entities/api_response.py
 pymino/ext/entities/bubble.py
```

### Comparing `pymino-1.2.1.9/setup.cfg` & `pymino-1.2.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e31 2e39 0d0a 6175  on = 1.2.1.9..au
+00000020: 6f6e 203d 2031 2e32 2e32 2e31 0d0a 6175  on = 1.2.2.1..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.1.9/setup.py` & `pymino-1.2.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,19 +14,20 @@
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/forevercynical/pymino",
     version = config.get('metadata', 'version'),
     packages=find_packages(),
     install_requires=[
         "requests==2.31.0",
-        "ujson==5.7.0",
+        "ujson==5.8.0",
         "colorama==0.4.6",
-        "websocket-client==1.5.2",
-        "diskcache==5.4.0",
-        "aiohttp==3.8.4"
+        "websocket-client==1.6.1",
+        "diskcache==5.6.1",
+        "aiohttp==3.8.4",
+        "wsaccel==0.6.4"
     ],
     keywords=[
         "amino",
         "pymino",
         "narvii",
         "amino-api",
         "narvii-bots",
```

