# Comparing `tmp/mentord-1.0.0.tar.gz` & `tmp/mentord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.0.0.tar", last modified: Tue Jun 27 09:51:15 2023, max compression
+gzip compressed data, was "mentord-1.0.1.tar", last modified: Tue Jun 27 09:58:25 2023, max compression
```

## Comparing `mentord-1.0.0.tar` & `mentord-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:51:15.025085 mentord-1.0.0/
--rw-rw-rw-   0        0        0       95 2023-06-27 09:51:15.026088 mentord-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 09:51:15.020570 mentord-1.0.0/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.0/mentord/__init__.py
--rw-rw-rw-   0        0        0     1666 2023-06-27 09:40:20.000000 mentord-1.0.0/mentord/channel.py
--rw-rw-rw-   0        0        0     2868 2023-06-27 09:40:16.000000 mentord-1.0.0/mentord/client.py
--rw-rw-rw-   0        0        0     1442 2023-06-27 08:08:34.000000 mentord-1.0.0/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.0/mentord/eother.py
--rw-rw-rw-   0        0        0     1119 2023-06-27 07:18:32.000000 mentord-1.0.0/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.0/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.0/mentord/member.py
--rw-rw-rw-   0        0        0      589 2023-06-27 09:27:26.000000 mentord-1.0.0/mentord/message.py
--rw-rw-rw-   0        0        0     1717 2023-06-27 09:40:33.000000 mentord-1.0.0/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:51:15.025085 mentord-1.0.0/mentord.egg-info/
--rw-rw-rw-   0        0        0       95 2023-06-27 09:51:14.000000 mentord-1.0.0/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 09:51:14.000000 mentord-1.0.0/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:51:14.000000 mentord-1.0.0/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 09:51:14.000000 mentord-1.0.0/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:51:15.027087 mentord-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      159 2023-06-27 09:51:09.000000 mentord-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:58:25.819064 mentord-1.0.1/
+-rw-rw-rw-   0        0        0       95 2023-06-27 09:58:25.820064 mentord-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 09:58:25.814066 mentord-1.0.1/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.1/mentord/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.1/mentord/channel.py
+-rw-rw-rw-   0        0        0     2872 2023-06-27 09:58:03.000000 mentord-1.0.1/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.1/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.1/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.1/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.1/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.1/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.1/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.1/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:58:25.819064 mentord-1.0.1/mentord.egg-info/
+-rw-rw-rw-   0        0        0       95 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:58:25.821064 mentord-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      159 2023-06-27 09:57:55.000000 mentord-1.0.1/setup.py
```

### Comparing `mentord-1.0.0/mentord/channel.py` & `mentord-1.0.1/mentord/channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from embed import *
-from http_ import *
-from member import *
-from message import *
+from .embed import *
+from .http_ import *
+from .member import *
+from .message import *
 
 
 class Channel:
 
     """
     Класс представляющий информацию о канале.
     """
```

### Comparing `mentord-1.0.0/mentord/client.py` & `mentord-1.0.1/mentord/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from threading import Thread
 
-from embed import *
-from http_ import *
-from message import *
-from user import *
+from .embed import *
+from .http_ import *
+from .message import *
+from .user import *
 
 
 class Client:
 
     """
     Класс выполняющий подключение с API.
     """
```

### Comparing `mentord-1.0.0/mentord/embed.py` & `mentord-1.0.1/mentord/embed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from eother import *
+from .eother import *
 
 
 class Embed:
 
     def __init__(self, description: str = "", author: Author = None, fields: list[Field] = [], title: str = "", url: str = None, image: Image = None, thumbnail: Thumbnail = None, footer: Footer = None, timestamp: str = ""):
 
         self.description: str = description
```

### Comparing `mentord-1.0.0/mentord/eother.py` & `mentord-1.0.1/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.0/mentord/guild.py` & `mentord-1.0.1/mentord/guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from http_ import *
-from member import *
+from .http_ import *
+from .member import *
 
 
 class Guild:
 
     """
     Класс представляющий информацию о гильдии.
     """
```

### Comparing `mentord-1.0.0/mentord/http_.py` & `mentord-1.0.1/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.0/mentord/member.py` & `mentord-1.0.1/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.0/mentord/message.py` & `mentord-1.0.1/mentord/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from member import *
+from .member import *
 
 class Message:
 
     def __init__(self, message: dict):
 
         self.message: dict = message
```

### Comparing `mentord-1.0.0/mentord/user.py` & `mentord-1.0.1/mentord/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from channel import *
-from guild import *
-from http_ import *
-from message import *
+from .channel import *
+from .guild import *
+from .http_ import *
+from .message import *
 
 
 class User:
 
     """
     Класс представляющий информацию о текущем подключенном объекте.
     """
```

