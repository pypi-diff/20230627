# Comparing `tmp/diself-1.0.1.tar.gz` & `tmp/diself-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diself-1.0.1.tar", last modified: Mon Jun 26 23:51:43 2023, max compression
+gzip compressed data, was "diself-1.0.2.tar", last modified: Tue Jun 27 14:05:19 2023, max compression
```

## Comparing `diself-1.0.1.tar` & `diself-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 23:51:43.206737 diself-1.0.1/
--rw-rw-rw-   0        0        0     1065 2023-06-26 22:08:08.000000 diself-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3203 2023-06-26 23:51:43.206737 diself-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2826 2023-06-26 23:10:20.000000 diself-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 23:51:43.201738 diself-1.0.1/diself/
--rw-rw-rw-   0        0        0       21 2023-06-26 23:28:11.000000 diself-1.0.1/diself/__init__.py
--rw-rw-rw-   0        0        0     4201 2023-06-26 23:51:21.000000 diself-1.0.1/diself/diself.py
-drwxrwxrwx   0        0        0        0 2023-06-26 23:51:43.205740 diself-1.0.1/diself.egg-info/
--rw-rw-rw-   0        0        0     3203 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 23:51:43.207738 diself-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-06-26 23:51:38.000000 diself-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:05:19.350638 diself-1.0.2/
+-rw-rw-rw-   0        0        0     1065 2023-06-26 22:08:08.000000 diself-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3202 2023-06-27 14:05:19.349638 diself-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2825 2023-06-27 14:01:04.000000 diself-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 14:05:19.345638 diself-1.0.2/diself/
+-rw-rw-rw-   0        0        0       21 2023-06-26 23:28:11.000000 diself-1.0.2/diself/__init__.py
+-rw-rw-rw-   0        0        0     4201 2023-06-26 23:51:21.000000 diself-1.0.2/diself/diself.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:05:19.349638 diself-1.0.2/diself.egg-info/
+-rw-rw-rw-   0        0        0     3202 2023-06-27 14:05:19.000000 diself-1.0.2/diself.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-27 14:05:19.000000 diself-1.0.2/diself.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:05:19.000000 diself-1.0.2/diself.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-27 14:05:19.000000 diself-1.0.2/diself.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 14:05:19.000000 diself-1.0.2/diself.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:05:19.350638 diself-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-06-27 14:00:35.000000 diself-1.0.2/setup.py
```

### Comparing `diself-1.0.1/LICENSE` & `diself-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diself-1.0.1/PKG-INFO` & `diself-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diself
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python module like discord.py but for selfbot
 Home-page: https://github.com/lululepu/diself
 Author: Lululepu
 Author-email: a.no.qsdf@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -52,15 +52,15 @@
 
 ## Usage
 
 ```python
 import diself
 
 @diself.event
-def on_messages(msg):
+def on_message(msg):
     print(msg) # print the raw message json
     print(msg.content) # print the message content
     print(msg.channel) # print the message channel
     print(msg.guild) # print the message guild
     chid=msg.channel # Get the channel
     message=chid.send("hey") # Send the message "key" to the channel
     message.delete() # Delete the message
```

### Comparing `diself-1.0.1/README.md` & `diself-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 ## Usage
 
 ```python
 import diself
 
 @diself.event
-def on_messages(msg):
+def on_message(msg):
     print(msg) # print the raw message json
     print(msg.content) # print the message content
     print(msg.channel) # print the message channel
     print(msg.guild) # print the message guild
     chid=msg.channel # Get the channel
     message=chid.send("hey") # Send the message "key" to the channel
     message.delete() # Delete the message
```

### Comparing `diself-1.0.1/diself/diself.py` & `diself-1.0.2/diself/diself.py`

 * *Files identical despite different names*

### Comparing `diself-1.0.1/diself.egg-info/PKG-INFO` & `diself-1.0.2/diself.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diself
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python module like discord.py but for selfbot
 Home-page: https://github.com/lululepu/diself
 Author: Lululepu
 Author-email: a.no.qsdf@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -52,15 +52,15 @@
 
 ## Usage
 
 ```python
 import diself
 
 @diself.event
-def on_messages(msg):
+def on_message(msg):
     print(msg) # print the raw message json
     print(msg.content) # print the message content
     print(msg.channel) # print the message channel
     print(msg.guild) # print the message guild
     chid=msg.channel # Get the channel
     message=chid.send("hey") # Send the message "key" to the channel
     message.delete() # Delete the message
```

