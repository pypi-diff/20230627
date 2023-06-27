# Comparing `tmp/mentord-1.0.1.tar.gz` & `tmp/mentord-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.0.1.tar", last modified: Tue Jun 27 09:58:25 2023, max compression
+gzip compressed data, was "mentord-1.0.2.tar", last modified: Tue Jun 27 10:06:54 2023, max compression
```

## Comparing `mentord-1.0.1.tar` & `mentord-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:58:25.819064 mentord-1.0.1/
--rw-rw-rw-   0        0        0       95 2023-06-27 09:58:25.820064 mentord-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 09:58:25.814066 mentord-1.0.1/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.1/mentord/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.1/mentord/channel.py
--rw-rw-rw-   0        0        0     2872 2023-06-27 09:58:03.000000 mentord-1.0.1/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.1/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.1/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.1/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.1/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.1/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.1/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.1/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:58:25.819064 mentord-1.0.1/mentord.egg-info/
--rw-rw-rw-   0        0        0       95 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 09:58:25.000000 mentord-1.0.1/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:58:25.821064 mentord-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      159 2023-06-27 09:57:55.000000 mentord-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:06:54.026118 mentord-1.0.2/
+-rw-rw-rw-   0        0        0       95 2023-06-27 10:06:54.027115 mentord-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 10:06:54.022118 mentord-1.0.2/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.2/mentord/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.2/mentord/channel.py
+-rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.2/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.2/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.2/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.2/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.2/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.2/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.2/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.2/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:06:54.026118 mentord-1.0.2/mentord.egg-info/
+-rw-rw-rw-   0        0        0       95 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:06:54.027115 mentord-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      159 2023-06-27 10:06:15.000000 mentord-1.0.2/setup.py
```

### Comparing `mentord-1.0.1/mentord/channel.py` & `mentord-1.0.2/mentord/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/client.py` & `mentord-1.0.2/mentord/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,14 @@
 
         messages: list[Message] = self.get_messages()
 
         while True:
 
             for channel in self.user.channels:
 
-                print(channel.id)
-
                 response = requests.get('https://discordapp.com/api/v9/channels/{0}/messages?after={1}&limit=5'.format(channel.id, messages[0].id),
                                         headers={"Authorization": self.user.token, "Content-Type": "application/json"}, )
 
                 if response.json().count != 0:
 
                     for message in response.json():
 
@@ -75,15 +73,15 @@
                         messages.insert(0, Message(message))
 
             time.sleep(1)
 
     def send_message(self, content: str = "", embeds: list[Embed] = [], channel_id: str = "") -> any:
 
         repsonse = HttpClient().request("POST", 'https://discordapp.com/api/v9//channels/{0}/messages'.format(channel_id),
-                                        header={"Authorization": self.token, "Content-Type": "application/json"}, json={
+                                        header={"Authorization": self.user.token, "Content-Type": "application/json"}, json={
             'content': content,
             'tts': False,
             'embeds': embeds
         })
 
         if repsonse.status_code != 200:
```

### Comparing `mentord-1.0.1/mentord/embed.py` & `mentord-1.0.2/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/eother.py` & `mentord-1.0.2/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/guild.py` & `mentord-1.0.2/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/http_.py` & `mentord-1.0.2/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/member.py` & `mentord-1.0.2/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/message.py` & `mentord-1.0.2/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.1/mentord/user.py` & `mentord-1.0.2/mentord/user.py`

 * *Files identical despite different names*

