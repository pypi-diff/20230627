# Comparing `tmp/pyrubi-2.1.1.tar.gz` & `tmp/pyrubi-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-2.1.1.tar", last modified: Sat Jun 10 10:56:52 2023, max compression
+gzip compressed data, was "pyrubi-2.2.0.tar", last modified: Tue Jun 27 14:34:12 2023, max compression
```

## Comparing `pyrubi-2.1.1.tar` & `pyrubi-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.158610 pyrubi-2.1.1/
--rw-rw-rw-   0        0        0     1935 2023-06-10 10:56:52.157610 pyrubi-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2023-06-10 10:50:53.000000 pyrubi-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.126635 pyrubi-2.1.1/pyrubi/
--rw-rw-rw-   0        0        0      246 2023-06-10 10:46:07.000000 pyrubi-2.1.1/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.143609 pyrubi-2.1.1/pyrubi/cryption/
--rw-rw-rw-   0        0        0     1194 2023-02-10 12:30:31.000000 pyrubi-2.1.1/pyrubi/cryption/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.144614 pyrubi-2.1.1/pyrubi/handler/
--rw-rw-rw-   0        0        0     1243 2023-06-07 06:58:02.000000 pyrubi-2.1.1/pyrubi/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.145614 pyrubi-2.1.1/pyrubi/maker/
--rw-rw-rw-   0        0        0     3164 2023-06-07 09:01:39.000000 pyrubi-2.1.1/pyrubi/maker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.145614 pyrubi-2.1.1/pyrubi/message/
--rw-rw-rw-   0        0        0     4687 2023-04-20 12:26:50.000000 pyrubi-2.1.1/pyrubi/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.146613 pyrubi-2.1.1/pyrubi/methods/
--rw-rw-rw-   0        0        0    43655 2023-06-07 09:00:36.000000 pyrubi-2.1.1/pyrubi/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.148612 pyrubi-2.1.1/pyrubi/servers/
--rw-rw-rw-   0        0        0      334 2023-05-26 15:37:31.000000 pyrubi-2.1.1/pyrubi/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.156611 pyrubi-2.1.1/pyrubi/tools/
--rw-rw-rw-   0        0        0     7100 2023-06-10 10:43:44.000000 pyrubi-2.1.1/pyrubi/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.141380 pyrubi-2.1.1/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 10:56:52.158610 pyrubi-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1116 2023-06-10 10:55:08.000000 pyrubi-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.288563 pyrubi-2.2.0/
+-rw-rw-rw-   0        0        0     2156 2023-06-27 14:34:12.288563 pyrubi-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1316 2023-06-27 14:31:50.000000 pyrubi-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.232560 pyrubi-2.2.0/pyrubi/
+-rw-rw-rw-   0        0        0      246 2023-06-27 14:18:29.000000 pyrubi-2.2.0/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.250135 pyrubi-2.2.0/pyrubi/cryption/
+-rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.2.0/pyrubi/cryption/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.251134 pyrubi-2.2.0/pyrubi/handler/
+-rw-rw-rw-   0        0        0     1142 2023-06-27 09:30:29.000000 pyrubi-2.2.0/pyrubi/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.259333 pyrubi-2.2.0/pyrubi/maker/
+-rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.2.0/pyrubi/maker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.261333 pyrubi-2.2.0/pyrubi/message/
+-rw-rw-rw-   0        0        0     4009 2023-06-27 13:19:11.000000 pyrubi-2.2.0/pyrubi/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.271329 pyrubi-2.2.0/pyrubi/methods/
+-rw-rw-rw-   0        0        0    45760 2023-06-27 13:43:21.000000 pyrubi-2.2.0/pyrubi/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.284752 pyrubi-2.2.0/pyrubi/servers/
+-rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.2.0/pyrubi/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.286028 pyrubi-2.2.0/pyrubi/sessions/
+-rw-rw-rw-   0        0        0      690 2023-06-27 12:19:25.000000 pyrubi-2.2.0/pyrubi/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.287560 pyrubi-2.2.0/pyrubi/tools/
+-rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.2.0/pyrubi/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.249184 pyrubi-2.2.0/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     2156 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:34:12.288563 pyrubi-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2023-06-27 14:32:51.000000 pyrubi-2.2.0/setup.py
```

### Comparing `pyrubi-2.1.1/PKG-INFO` & `pyrubi-2.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.1.1
+Version: 2.2.0
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir,bot
+Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.1.1</h1>
+<h1>Pyrubi 2.2.0</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.1' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.0' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
+**The Pyrubi library is compatible with version 6 of the Rubik's API**
+
+<hr>
+
+## Install or Update:
+
+``` bash
+pip install -U pyrubi
+```
+
 <hr>
 
-**Example:**
+## Example:
+
 ``` python
-from pyrubi import Bot, Message
+from pyrubi import Bot
 
-bot = Bot("TOKEN")
+bot = Bot("session")
 
 for update in bot.on_message():
-    message = Message(update)
-    if message.text() == 'hello':
-        bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://example.com).", message.message_id())
+    if update.text() == 'hello':
+        bot.send_text(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi library.__", update.message_id())
 ```
 
 <hr>
 
-### Features:
+## Features:
     
 - **Fast** : *The requests are very fast.*
 
 - **Easy** : *All methods and features are designed as easy and optimal as possible*
 
 - **Powerful** : *While the library is simple, it has high speed and features that make your work easier and faster*
 
 
 <hr>
 
-## Rubika : @pyrubika
+## Social Media:
+### <a href='https://rubika.ir/pyrubika'>Rubika</a>
 
-### Install or Update:
+<hr>
 
-``` bash
-pip install -U pyrubi
-```
+## 🌟 Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=AliGanji1/Pyrubi&type=Date)](https://star-history.com/#AliGanji1/Pyrubi&Date)
```

#### html2text {}

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.1.1 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.2.0 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
-ali.ganji.za@gmail.com Keywords: rubika,rubika-
-bot,pyrubi,rubx,rubino,rubika.ir,bot Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
-Python: ~=3.6 Description-Content-Type: text/markdown
-****** Pyrubi 2.1.1 ******
+ali.ganji.za@gmail.com Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
+markdown
+****** Pyrubi 2.2.0 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.1.1]
+                            [Pyrubi Library 2.2.0]
                              GitHub â¢ Documents
+**The Pyrubi library is compatible with version 6 of the Rubik's API**
 ===============================================================================
-**Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
-update in bot.on_message(): message = Message(update) if message.text() ==
-'hello': bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title
-()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://
-example.com).", message.message_id()) ```
+## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
-### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
+## Example: ``` python from pyrubi import Bot bot = Bot("session") for update
+in bot.on_message(): if update.text() == 'hello': bot.send_text(update.chat_id
+(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi
+library.__", update.message_id()) ```
+===============================================================================
+## Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
-## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
+## Social Media: ### Rubika
+===============================================================================
+## ð Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=AliGanji1/Pyrubi&type=Date)](https://star-history.com/#AliGanji1/
+Pyrubi&Date)
```

### Comparing `pyrubi-2.1.1/README.md` & `pyrubi-2.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,59 @@
-<h1>Pyrubi 2.1.1</h1>
+<h1>Pyrubi 2.2.0</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.1' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.0' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
+**The Pyrubi library is compatible with version 6 of the Rubik's API**
+
+<hr>
+
+## Install or Update:
+
+``` bash
+pip install -U pyrubi
+```
+
 <hr>
 
-**Example:**
+## Example:
+
 ``` python
-from pyrubi import Bot, Message
+from pyrubi import Bot
 
-bot = Bot("TOKEN")
+bot = Bot("session")
 
 for update in bot.on_message():
-    message = Message(update)
-    if message.text() == 'hello':
-        bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://example.com).", message.message_id())
+    if update.text() == 'hello':
+        bot.send_text(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi library.__", update.message_id())
 ```
 
 <hr>
 
-### Features:
+## Features:
     
 - **Fast** : *The requests are very fast.*
 
 - **Easy** : *All methods and features are designed as easy and optimal as possible*
 
 - **Powerful** : *While the library is simple, it has high speed and features that make your work easier and faster*
 
 
 <hr>
 
-## Rubika : @pyrubika
+## Social Media:
+### <a href='https://rubika.ir/pyrubika'>Rubika</a>
 
-### Install or Update:
+<hr>
 
-``` bash
-pip install -U pyrubi
-```
+## 🌟 Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=AliGanji1/Pyrubi&type=Date)](https://star-history.com/#AliGanji1/Pyrubi&Date)
```

#### html2text {}

```diff
@@ -1,17 +1,23 @@
-****** Pyrubi 2.1.1 ******
+****** Pyrubi 2.2.0 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.1.1]
+                            [Pyrubi Library 2.2.0]
                              GitHub â¢ Documents
+**The Pyrubi library is compatible with version 6 of the Rubik's API**
 ===============================================================================
-**Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
-update in bot.on_message(): message = Message(update) if message.text() ==
-'hello': bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title
-()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://
-example.com).", message.message_id()) ```
+## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
-### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
+## Example: ``` python from pyrubi import Bot bot = Bot("session") for update
+in bot.on_message(): if update.text() == 'hello': bot.send_text(update.chat_id
+(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi
+library.__", update.message_id()) ```
+===============================================================================
+## Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
-## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
+## Social Media: ### Rubika
+===============================================================================
+## ð Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=AliGanji1/Pyrubi&type=Date)](https://star-history.com/#AliGanji1/
+Pyrubi&Date)
```

### Comparing `pyrubi-2.1.1/pyrubi/cryption/__init__.py` & `pyrubi-2.2.0/pyrubi/handler/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from Crypto.Util.Padding import pad, unpad
-from base64 import b64encode as b64e, urlsafe_b64decode as b64d
-from Crypto.Cipher import AES
+from websocket import create_connection
+from json import dumps, loads
+from ..servers import get_server
+from ..cryption import cryption5
+class handler:
 
-class cryption:
-    
     def __init__(self, auth):
-        self.key = bytearray(self.secret(auth), 'UTF-8')
-        self.iv = bytearray.fromhex('0' * 32)
-        
-    def replaceCharAt(self, e, t, i):
-        return e[0:t] + i + e[t + len(i):]
-
-    def secret(self, e):
-        t, n, s = e[0:8], e[16:24] + e[0:8] + e[24:32] + e[8:16], 0
-        while s < len(n):
-            e = n[s]
-            if e >= '0' and e <= '9':
-                t = chr((ord(e[0]) - ord('0') + 5) %10 + ord('0'))
-                n = self.replaceCharAt(n, s, t)
-            else:
-                t = chr((ord(e[0]) - ord('a') + 9) %26 + ord('a'))
-                n = self.replaceCharAt(n, s, t)
-            s += 1
-        return n
-
-    def encrypt(self, text):
-        return b64e(AES.new(self.key, AES.MODE_CBC, self.iv).encrypt(pad(text.encode('UTF-8'), AES.block_size))).decode('UTF-8')
-
-    def decrypt(self, text):
-        return unpad(AES.new(self.key, AES.MODE_CBC, self.iv).decrypt(b64d(text.encode('UTF-8'))), AES.block_size).decode('UTF-8')
+        self.crypto = cryption5(auth) if auth else None
+        self.auth = auth
+        self.hs_data = {
+            'api_version': '5',
+            'auth': auth,
+            'method': 'handShake'
+        }
+        del auth
+    
+    def hand_shake(self):
+        print('connecting to the web socket...')
+        ws = create_connection(get_server('socket'))
+        ws.send(dumps(self.hs_data))
+        print('connected !')
+        while True:
+            try:
+                recv = loads(ws.recv())
+                if recv != {"status":"OK", "status_det":"OK"}:
+                    if recv['type'] == 'messenger':
+                        yield loads(self.crypto.decrypt(recv['data_enc']))
+            except:
+                ws.close()
+                del ws
+                ws = create_connection(self.server)
+                print(self.methods.get_me())
+                ws.send(dumps(self.hs_data))
+                continue
```

### Comparing `pyrubi-2.1.1/pyrubi/maker/__init__.py` & `pyrubi-2.2.0/pyrubi/maker/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,78 @@
-from ..cryption import cryption
 from ..servers import get_server
 from urllib3 import PoolManager
 from json import dumps, loads
 from requests import  post
 
 class maker:
     
-    def __init__(self, auth, methods):
-        self.auth = auth
-        self.crypto = cryption(auth)
+    def __init__(self, send_auth, crypto):
+        self.auth = send_auth
+        self.crypto = crypto
         self.http = PoolManager()
         self.server = get_server('api')
-        self.methods = methods
         self.req_clients = {
             'web': {
-                'app_name':'Main',
-                'app_version':'4.2.0',
-                'platform':'Web',
-                'package':'web.rubika.ir',
-                'lang_code':'fa'
+                'app_name': 'Main',
+                'app_version': '4.3.3',
+                'platform': 'Web',
+                'package': 'web.rubika.ir',
+                'lang_code': 'fa'
             },
             'android': {
                 'app_name': 'Main',
-                'app_version': '3.0.9',
+                'app_version': '3.3.2',
                 'platform': 'Android',
                 'package': 'ir.resaneh1.iptv',
                 'lang_code': 'fa'
             }
         }
-        del auth
+        self.raise_info = {
+            'INVALID_AUTH': 'The Auth entered is invalid !',
+            'NOT_REGISTERED': 'Method input is not registered !',
+            'INVALID_INPUT': 'Invalid method input !',
+            'TOO_REQUESTS': 'Too much request ! Your account has been suspended.'
+        }
+        del send_auth
 
-    def method(self, method, data, api_version=5):
+    def method(self, method:str, data:dict, tmp:str=None, api_version:int=6):
+        if tmp:
+            from ..cryption import cryption6
+            self.crypto = cryption6(tmp)
         data = {
             'api_version': str(api_version),
-            'auth': self.auth,
+            'tmp_session' if tmp else 'auth': tmp if tmp else self.auth,
             'data_enc': self.crypto.encrypt(
-                dumps(
-                    {
-                        'method': method,
-                        'input': data,
-                        'client': self.req_clients['web']
-                    }
-                )
+                dumps({
+                    'method': method,
+                    'input': data,
+                    'client': self.req_clients['web']
+                })
             )
         }
-        trying = 0
+        if str(api_version) == "6" and not tmp:
+            data['sign'] = self.crypto.makeSignFromData(data['data_enc'])
+
         while True:
             result = self.http.request(
                 'POST',
                 self.server,
+                headers={
+                    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+                    'Origin': 'https://web.rubika.ir',
+					'Referer': 'https://web.rubika.ir/',
+					'Host': self.server.replace('https://','').replace('/','')
+                },
                 body = dumps(data).encode(),
             )
-            result = loads(self.crypto.decrypt(loads(result.data.decode('utf-8'))['data_enc']))
+            result = loads(self.crypto.decrypt(loads(result.data.decode('UTF-8'))['data_enc']))
             if result['status'] == 'OK':
                 return result['data']
             elif result['status'] in ['ERROR_GENERIC', 'ERROR_ACTION']:
-                if result['status_det'] == 'INVALID_AUTH':
-                    if trying < 3:
-                        self.methods.get_me()
-                        trying += 1
-                        continue
-                    raise ConnectionError('The Auth entered is invalid !')
-                for i in [
-                    ('NOT_REGISTERED', 'Method input is not registered !'),
-                    ('INVALID_INPUT', 'Invalid method input !'),
-                    ('TOO_REQUESTS', 'Too much request ! Your account has been suspended.')
-                ]: 
-                    if result['status_det'] == i[0]:
-                        raise ConnectionError(i[1])
+                raise ConnectionError(self.raise_info[result['status_det']])
             continue
 
     def _upload(self, url, data, headers):
         while True:
             req = post(url=url, data=data, headers=headers)
             if req.status_code != 200:
                 print('This file cannot be uploaded ! Trying to upload again ...')
```

### Comparing `pyrubi-2.1.1/pyrubi/methods/__init__.py` & `pyrubi-2.2.0/pyrubi/methods/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,86 @@
-from ..cryption import cryption
+from ..sessions import sessions
+from ..cryption import cryption6
 from ..tools import tools
 from ..message import message
 from ..maker import maker
 from ..handler import handler
 from requests import session
 from urllib3 import PoolManager
 from random import choice, randint
 from time import time
 from pathlib import Path
 
 class methods:
 
-    def __init__(self, auth):
-        self.auth = auth
-        self.hs = handler(auth, self).hand_shake
-        self.method = maker(auth, self).method
-        self.crypto = cryption(auth)
+    def __init__(self, session:str):
+        if sessions.cheack_session(session):
+            self.session_data = sessions.session_data(session)
+        else:
+            self.method = maker(None, cryption6).method
+            self.session_data = self.create_session(session, input("Enter the phone number: "))
+
+        self.crypto = cryption6(self.session_data['auth'], self.session_data['private_key'])
+        self.hs = handler(self.session_data['auth']).hand_shake
+        self.method = maker(cryption6.changeAuthType(self.session_data['auth']), self.crypto).method
         self.http = PoolManager()
         self.got_messages_update = []
-        del auth
 
+    def create_session(self, session_name, phone_number:str):
+        send_code_data = self.send_code(phone_number)
+
+        if send_code_data[0]['status'] == 'SendPassKey':
+            pass_key = input(f'Enter the pass key({send_code_data[0]["hint_pass_key"]}): ')
+            send_code_data = self.send_code(phone_number, pass_key)
+        
+        if send_code_data[0]['status'] == 'InvalidPassKey':
+            return print(f'Pass key({send_code_data[0]["hint_pass_key"]}) is invalid!')
+        
+        input_code = input("Enter the code: ").strip()
+
+        sign_in_data = self.sign_in(phone_number, send_code_data[0]['phone_code_hash'], input_code, send_code_data[1])
+
+        if sign_in_data[0]['status'] == 'OK':
+
+            session_data = {
+                'auth': cryption6.decryptRsaOaep(sign_in_data[1], sign_in_data[0]['auth']),
+                'private_key': sign_in_data[1],
+                'user': sign_in_data[0]['user'],
+            }
+
+            sessions.create_session(session_name, session_data)
+
+            methods(session_name).register_device(
+                "Windows 10",
+                f"Pyrubi Library | {session_name}",
+                "25010064641090201001011130"
+            )
+
+            print(f"\nAUTH: '{session_data['auth']}'\nPRIVATE KEY: '{sign_in_data[1]}'\n")
+
+            return session_data
+        
+        return sign_in_data
 
     def on_message(self, chat_filter=[], message_filter=[]):
         for recv in self.hs():
-            if 'chat_updates' in recv and not message(recv).chat_type() in chat_filter and not message(recv).message_type() in message_filter:
-                yield recv
-            else:
-                continue
+            if 'chat_updates' in recv.keys() and recv["message_updates"]:
+                msg = message(recv)
+                if not msg.chat_type() in chat_filter and not msg.message_type() in message_filter:
+                    yield msg
 
-    def get_chats_update(self, chat_filter=[], message_filter=[], save_message_ids=True):
+    def get_chats_update(self, chat_filter=[], message_filter=[]):
         while True:
             try:
+                msg = message(chats_update)
                 chats_update = self.method('getChatsUpdates', {'state': round(time()) - 200})['chats'][0]
-                if not message(chats_update).chat_type() in chat_filter and not message(chats_update).message_type() in message_filter:
-                    if save_message_ids:
-                        if not message(chats_update).message_id() in self.got_messages_update:
-                            self.got_messages_update.append(message(chats_update).message_id())
-                            yield chats_update
-                    else:
-                        yield chats_update
+                if not msg.chat_type() in chat_filter and not msg.message_type() in message_filter:
+                    if not msg.message_id() in self.got_messages_update:
+                        self.got_messages_update.append(msg.message_id())
+                        yield msg
             except IndexError:
                 continue
 
     def get_chats_update2(self):
         return self.method('getChatsUpdates', {'state': round(time()) - 200})['chats']
 
     def send_text(self, chat_id, text, message_id = None):
@@ -751,23 +789,26 @@
 
     def get_contacts_updates(self, state):
         return self.method('getContactsUpdates', {'state': state})
 
     def get_contacts_last_online(self, chat_ids : list = None):
         return self.method('getContactsLastOnline', {'user_guds': chat_ids})
 
-    def add_contact(self, phone_number, first_name, last_name):
+    def add_contact(self, phone_number, first_name, last_name=""):
         return self.method(
             'addAddressBook',
             {
                 'phone': f'98{tools.parse_phone_number(phone_number)}',
                 'first_name': first_name,
                 'last_name': last_name
             }
         )
+    
+    def delete_contact(self, user_id):
+        return self.method('deleteContact', {'user_guid': user_id})
 
     def get_folders(self):
         return self.method('getFolders', {})
 
     def get_suggested_folders(self):
         return self.method('getSuggestedFolders', {})
 
@@ -836,42 +877,25 @@
             }            
         )
     
     def get_sticker_sets(self):
         return self.method('getMyStickerSets', {})
 
     def get_me(self):
-        session().close()
-        return session().post(
-            'https://messengerg2c1.iranlms.ir',
-            json={
-                "data":{},
-                "method":"getUser",
-                "api_version":"2",
-                "auth": self.auth,
-                "Messenger":{
-                    "app_name":"Main",
-                    "package":"m.rubika.ir",
-                    "app_version":"1.2.1",
-                    "platform":"PWA"
-                }
-            },
-            headers = {
-                'referer': 'https://web.rubika.ir/',
-            }
-        ).json()
+        self.session_data['user'] = self.get_chat_info(self.session_data['user']['user_guid'])['user']
+        return self.session_data
     
     def get_base_info(self):
         return session().post(
             'https://servicesbase.iranlms.ir/',
             json={
                 'method':'getBaseInfo',
                 'api_version':'0',
                 'data':{},
-                'auth': self.auth,
+                'auth': self.session_data['auth'],
                 'client':{
                     'app_name':'Main',
                     'app_version':'4.2.0',
                     'platform':'PWA',
                     'package':'web.rubika.ir'
                 }
             }
@@ -880,15 +904,15 @@
     def get_tag_list(self):
         return session().post(
             'https://services3.iranlms.ir/',
             json={
                 'method':'getTagList',
                 'api_version':'0',
                 'data':{'taglist_id': 'new_vod'},
-                'auth': self.auth,
+                'auth': self.session_data['auth'],
                 'client':{
                     'app_name':'Main',
                     'app_version':'4.2.0',
                     'platform':'PWA',
                     'package':'web.rubika.ir'
                 }
             }
@@ -935,30 +959,50 @@
                     'Everybody' if link_forward_message else 'Nobody',
                     'Everybody' if can_join_chat else 'Nobody'
                 ]
             }
         )
 
     def send_code(self, phone_number, pass_key=None, send_internal=False):
+        tmp = tools.make_random_tmp_session()
         return self.method(
             'sendCode',
             {
                 'phone_number': f'98{tools.parse_phone_number(phone_number)}',
                 'send_type': 'Internal' if send_internal else 'SMS',
                 'pass_key': pass_key
-            }
-        )
+            },
+            tmp
+        ), tmp
+
+    def sign_in(self, phone_number, phone_code_hash, phone_code, tmp, public_key=None):
+        public, private = cryption6.rsaKeyGenrate()
 
-    def sing_in(self, phone_number, phone_code_hash, phone_code):
         return self.method(
             'signIn',
             {
                 'phone_number': f'98{tools.parse_phone_number(phone_number)}',
                 'phone_code_hash': phone_code_hash,
-                'phone_code': phone_code
+                'phone_code': phone_code,
+			    "public_key": public_key or public
+            },
+            tmp
+        ), private
+    
+    def register_device(self, systemversion, device_model, device_hash):
+        return self.method(
+            'registerDevice',
+            {
+                'token_type': 'Web',
+                'token': '',
+                'app_version': 'WB_4.3.3',
+                'lang_code': 'fa',
+                'system_version': systemversion,
+                'device_model': device_model,
+                'device_hash': device_hash
             }
         )
 
     def logout(self):
         return self.method('logout', {})
     
     def get_chat_ads(self):
@@ -980,20 +1024,20 @@
             }
         ), url_data
 
     def upload_file(self, file):
         req = self.request_file(file)
         file_data = req[0]
         url_data = req[1]
-        upload = maker(self.auth, self)._upload
+        upload = maker(self.session_data['auth'], self.crypto)._upload
         bytef = url_data.data if url_data else file if str(type(file)) == "<class 'bytes'>" else open(file,'rb').read()
         size = str(len(url_data.data)) if url_data else str(len(file)) if str(type(file)) == "<class 'bytes'>" else str(Path(file).stat().st_size)
         url = file_data['upload_url']
         header = {
-            'auth': self.auth,
+            'auth': self.session_data['auth'],
             'Host': file_data['upload_url'].replace('https://','').replace('/UploadFile.ashx',''),
             'chunk-size': size,
             'data-length': size,
             'file-id': str(file_data['id']),
             'access-hash-send': file_data['access_hash_send'],
             'data-type': 'application/octet-stream',
         }
@@ -1019,23 +1063,23 @@
             
     def download_file(self, chat_id=None, message_id=None, save=False, file_inline=None):
         message_data = file_inline if file_inline else self.get_messages_info(chat_id, [message_id])[0].get('file_inline', None)
         if not message_data:
             raise FileExistsError(f'This ({message_id}) message is not a File !')
         file_name = message_data.get('file_name', f'pyrubi {time()}.{message_data.get("mime", "pyrubi")}')
         header = {
-            'auth': self.auth,
+            'auth': self.session_data['auth'],
             'file-id': str(message_data['file_id']),
             'access-hash-rec': message_data['access_hash_rec'],
             'client-app-version': '3.1.1',
             'client-platform': 'Android',
             'client-app-name': 'Main',
             'client-package': 'app.rbmain.a'
         }
-        download = maker(self.auth)._download
+        download = maker(self.session_data['auth'], self.crypto)._download
         response = download(f'https://messenger{message_data["dc_id"]}.iranlms.ir/GetFile.ashx', header)
         chunk = b''
         for i in response.stream(524284):
             chunk += i
             print('\r' + f'{round(len(chunk) / 1024) / 1000} MB /', sep='', end=f' {message_data["size"] / 1000000} MB' if 'size' in message_data else None)
         if save:
             with open(file_name, 'wb+') as file:
```

### Comparing `pyrubi-2.1.1/pyrubi/tools/__init__.py` & `pyrubi-2.2.0/pyrubi/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from random import randint
+from random import randint, choice
 from requests import get
 from base64 import b64encode as b64e
 from PIL import Image
 from io import BytesIO
 from mutagen.mp3 import MP3
 from tinytag import TinyTag
 from re import finditer
@@ -182,8 +182,15 @@
     def parse_phone_number(phone_number):
         if str(phone_number).startswith('0'):
             phone_number = phone_number[1:]
         elif str(phone_number).startswith('98'):
             phone_number = phone_number[2:]
         elif str(phone_number).startswith('+98'):
             phone_number = phone_number[3:]
-        return phone_number
+        return phone_number
+    
+    def make_random_tmp_session():
+        chars = "abcdefghijklmnopqrstuvwxyz"
+        tmp = ""
+        for i in range(32):
+            tmp += choice(chars)
+        return tmp
```

### Comparing `pyrubi-2.1.1/pyrubi.egg-info/PKG-INFO` & `pyrubi-2.2.0/pyrubi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.1.1
+Version: 2.2.0
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir,bot
+Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.1.1</h1>
+<h1>Pyrubi 2.2.0</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.1' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.0' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
+**The Pyrubi library is compatible with version 6 of the Rubik's API**
+
+<hr>
+
+## Install or Update:
+
+``` bash
+pip install -U pyrubi
+```
+
 <hr>
 
-**Example:**
+## Example:
+
 ``` python
-from pyrubi import Bot, Message
+from pyrubi import Bot
 
-bot = Bot("TOKEN")
+bot = Bot("session")
 
 for update in bot.on_message():
-    message = Message(update)
-    if message.text() == 'hello':
-        bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://example.com).", message.message_id())
+    if update.text() == 'hello':
+        bot.send_text(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi library.__", update.message_id())
 ```
 
 <hr>
 
-### Features:
+## Features:
     
 - **Fast** : *The requests are very fast.*
 
 - **Easy** : *All methods and features are designed as easy and optimal as possible*
 
 - **Powerful** : *While the library is simple, it has high speed and features that make your work easier and faster*
 
 
 <hr>
 
-## Rubika : @pyrubika
+## Social Media:
+### <a href='https://rubika.ir/pyrubika'>Rubika</a>
 
-### Install or Update:
+<hr>
 
-``` bash
-pip install -U pyrubi
-```
+## 🌟 Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=AliGanji1/Pyrubi&type=Date)](https://star-history.com/#AliGanji1/Pyrubi&Date)
```

#### html2text {}

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.1.1 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.2.0 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
-ali.ganji.za@gmail.com Keywords: rubika,rubika-
-bot,pyrubi,rubx,rubino,rubika.ir,bot Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
-Python: ~=3.6 Description-Content-Type: text/markdown
-****** Pyrubi 2.1.1 ******
+ali.ganji.za@gmail.com Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
+markdown
+****** Pyrubi 2.2.0 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.1.1]
+                            [Pyrubi Library 2.2.0]
                              GitHub â¢ Documents
+**The Pyrubi library is compatible with version 6 of the Rubik's API**
 ===============================================================================
-**Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
-update in bot.on_message(): message = Message(update) if message.text() ==
-'hello': bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title
-()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://
-example.com).", message.message_id()) ```
+## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
-### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
+## Example: ``` python from pyrubi import Bot bot = Bot("session") for update
+in bot.on_message(): if update.text() == 'hello': bot.send_text(update.chat_id
+(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi
+library.__", update.message_id()) ```
+===============================================================================
+## Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
-## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
+## Social Media: ### Rubika
+===============================================================================
+## ð Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=AliGanji1/Pyrubi&type=Date)](https://star-history.com/#AliGanji1/
+Pyrubi&Date)
```

### Comparing `pyrubi-2.1.1/setup.py` & `pyrubi-2.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrubi',
-    version = '2.1.1',
+    version = '2.2.0',
     author='Ali Ganji zadeh',
     author_email = 'ali.ganji.za@gmail.com',
     description = 'This is a powerful and easy library for building self Bots in Rubika',
-    keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubx', 'rubino', 'rubika.ir', 'bot'],
+    keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubx', 'rubino', 'rubika.ir'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/AliGanji1/pyrubi',
     packages = find_packages(),
     install_requires = ['pycryptodome', 'websocket-client', 'requests', 'urllib3', 'pillow', 'mutagen', 'tinytag'],
     classifiers = [
```

