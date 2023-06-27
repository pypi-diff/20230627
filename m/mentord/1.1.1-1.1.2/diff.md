# Comparing `tmp/mentord-1.1.1.tar.gz` & `tmp/mentord-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.1.tar", last modified: Tue Jun 27 11:13:18 2023, max compression
+gzip compressed data, was "mentord-1.1.2.tar", last modified: Tue Jun 27 12:55:39 2023, max compression
```

## Comparing `mentord-1.1.1.tar` & `mentord-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:13:18.443517 mentord-1.1.1/
--rw-rw-rw-   0        0        0      391 2023-06-27 11:13:18.444605 mentord-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 11:13:18.438517 mentord-1.1.1/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.1.1/mentord/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.1.1/mentord/channel.py
--rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.1.1/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.1.1/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.1.1/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.1.1/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.1.1/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.1.1/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.1.1/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.1.1/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:13:18.443517 mentord-1.1.1/mentord.egg-info/
--rw-rw-rw-   0        0        0      391 2023-06-27 11:13:18.000000 mentord-1.1.1/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 11:13:18.000000 mentord-1.1.1/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:13:18.000000 mentord-1.1.1/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 11:13:18.000000 mentord-1.1.1/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 11:13:18.445605 mentord-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      496 2023-06-27 11:12:48.000000 mentord-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:55:39.712671 mentord-1.1.2/
+-rw-rw-rw-   0        0        0      391 2023-06-27 12:55:39.713670 mentord-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 12:55:39.707575 mentord-1.1.2/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.1.2/mentord/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.1.2/mentord/channel.py
+-rw-rw-rw-   0        0        0     2884 2023-06-27 12:55:25.000000 mentord-1.1.2/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.1.2/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.1.2/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.1.2/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.1.2/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.1.2/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.1.2/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.1.2/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:55:39.711672 mentord-1.1.2/mentord.egg-info/
+-rw-rw-rw-   0        0        0      391 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 12:55:39.000000 mentord-1.1.2/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:55:39.713670 mentord-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      496 2023-06-27 12:55:33.000000 mentord-1.1.2/setup.py
```

### Comparing `mentord-1.1.1/mentord/channel.py` & `mentord-1.1.2/mentord/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/client.py` & `mentord-1.1.2/mentord/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,42 +39,42 @@
 
             time.sleep(0.5)
 
         func()
         new_t = Thread(target=self.connect_stable)
         new_t.start()
 
-    def get_messages(self) -> list[Message]:
+    def get_messages_id(self) -> dict:
 
-        messages: list[Message] = []
+        messages: dict = {}
 
         for channel in self.user.channels:
-
-            messages += channel.messages
-
+            
+            messages[channel.id] = channel.messages[0].id
+        
         return messages
 
     def message_processing(self, func):
 
-        messages: list[Message] = self.get_messages()
+        messages: dict = self.get_messages_id()
 
         while True:
 
             for channel in self.user.channels:
 
-                response = requests.get('https://discordapp.com/api/v9/channels/{0}/messages?after={1}&limit=5'.format(channel.id, messages[0].id),
+                response = requests.get('https://discordapp.com/api/v9/channels/{0}/messages?after={1}&limit=1'.format(channel.id, messages[channel.id]),
                                         headers={"Authorization": self.user.token, "Content-Type": "application/json"}, )
 
                 if response.json().count != 0:
 
                     for message in response.json():
 
                         func(Message(message))
-
-                        messages.insert(0, Message(message))
+                
+                        messages[channel.id] = Message(message).id
 
             time.sleep(1)
 
     def send_message(self, content: str = "", embeds: list[Embed] = [], channel_id: str = "") -> any:
 
         repsonse = HttpClient().request("POST", 'https://discordapp.com/api/v9//channels/{0}/messages'.format(channel_id),
                                         header={"Authorization": self.user.token, "Content-Type": "application/json"}, json={
```

### Comparing `mentord-1.1.1/mentord/embed.py` & `mentord-1.1.2/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/eother.py` & `mentord-1.1.2/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/guild.py` & `mentord-1.1.2/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/http_.py` & `mentord-1.1.2/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/member.py` & `mentord-1.1.2/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/message.py` & `mentord-1.1.2/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.1/mentord/user.py` & `mentord-1.1.2/mentord/user.py`

 * *Files identical despite different names*

