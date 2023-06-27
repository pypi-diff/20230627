# Comparing `tmp/mentord-1.1.2.tar.gz` & `tmp/mentord-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.2.tar", last modified: Tue Jun 27 12:55:39 2023, max compression
+gzip compressed data, was "mentord-1.1.3.tar", last modified: Tue Jun 27 13:17:47 2023, max compression
```

## Comparing `mentord-1.1.2.tar` & `mentord-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:55:39.712671 mentord-1.1.2/
--rw-rw-rw-   0        0        0      391 2023-06-27 12:55:39.713670 mentord-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 12:55:39.707575 mentord-1.1.2/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.1.2/mentord/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.1.2/mentord/channel.py
--rw-rw-rw-   0        0        0     2884 2023-06-27 12:55:25.000000 mentord-1.1.2/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.1.2/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.1.2/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.1.2/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.1.2/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.1.2/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.1.2/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.1.2/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:55:39.711672 mentord-1.1.2/mentord.egg-info/
--rw-rw-rw-   0        0        0      391 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 12:55:39.713670 mentord-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      496 2023-06-27 12:55:33.000000 mentord-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:17:47.241837 mentord-1.1.3/
+-rw-rw-rw-   0        0        0      612 2023-06-27 13:17:47.241837 mentord-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 13:17:47.236314 mentord-1.1.3/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 13:13:33.000000 mentord-1.1.3/mentord/__init__.py
+-rw-rw-rw-   0        0        0     2107 2023-06-27 12:58:51.000000 mentord-1.1.3/mentord/channel.py
+-rw-rw-rw-   0        0        0     2884 2023-06-27 12:55:25.000000 mentord-1.1.3/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.1.3/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.1.3/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.1.3/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.1.3/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.1.3/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.1.3/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.1.3/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:17:47.240838 mentord-1.1.3/mentord.egg-info/
+-rw-rw-rw-   0        0        0      612 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:17:47.242836 mentord-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      717 2023-06-27 13:17:38.000000 mentord-1.1.3/setup.py
```

### Comparing `mentord-1.1.2/mentord/channel.py` & `mentord-1.1.3/mentord/channel.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,40 +14,60 @@
 
         self.channel: dict = channel
         self.token: str = token
 
     @property
     def id(self) -> str:
 
+        """
+        Id канала.
+        """
+
         return str(self.channel['id'])
 
     @property
     def member(self) -> Member:
 
+        """
+        Соучастник канала.
+        """
+
         return Member(self.channel['recipients'][0])
     
     @property
     def messages(self) -> list[Message]:
         
+        """
+        Получение некоторых сообщений из канала.
+        """
+
         user_messages: list[Message] = []
 
         for message in HttpClient().request("GET", 'https://discordapp.com/api/v9/channels/{0}/messages'.format(self.id),
                                             {"Authorization": self.token, "Content-Type": "application/json"}).json():
 
             user_messages.append(Message(message))
 
         return user_messages
 
 
     def get_json_object(self) -> dict:
 
+        """
+        Получить объект в виде словаря.
+        """
+
         return self.channel
     
     def send_message(self, content: str = "", embeds: list[Embed] = []) -> any:
 
+        """
+        Отправить сообщение в данный канал.
+        """
+
         repsonse = HttpClient().request("POST", 'https://discordapp.com/api/v9//channels/{0}/messages'.format(self.id),
                             header={"Authorization": self.token, "Content-Type": "application/json"}, json={
                                 'content': content,
                                 'tts': False,
                                 'embeds': embeds
                                 })
```

### Comparing `mentord-1.1.2/mentord/client.py` & `mentord-1.1.3/mentord/client.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/embed.py` & `mentord-1.1.3/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/eother.py` & `mentord-1.1.3/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/guild.py` & `mentord-1.1.3/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/http_.py` & `mentord-1.1.3/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/member.py` & `mentord-1.1.3/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/message.py` & `mentord-1.1.3/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.2/mentord/user.py` & `mentord-1.1.3/mentord/user.py`

 * *Files identical despite different names*

