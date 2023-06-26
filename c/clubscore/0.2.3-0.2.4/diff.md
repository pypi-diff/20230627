# Comparing `tmp/clubscore-0.2.3.tar.gz` & `tmp/clubscore-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clubscore-0.2.3.tar", last modified: Sat Jun 24 15:34:53 2023, max compression
+gzip compressed data, was "clubscore-0.2.4.tar", last modified: Mon Jun 26 23:43:55 2023, max compression
```

## Comparing `clubscore-0.2.3.tar` & `clubscore-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.275006 clubscore-0.2.3/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.2.3/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-24 15:34:53.274412 clubscore-0.2.3/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.2.3/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.261828 clubscore-0.2.3/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)     1206 2023-06-24 15:29:38.000000 clubscore-0.2.3/clubscore/API.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.3/clubscore/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     5159 2023-06-24 13:56:51.000000 clubscore-0.2.3/clubscore/bot.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.272076 clubscore-0.2.3/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     5435 2023-06-24 11:41:29.000000 clubscore-0.2.3/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     3171 2023-06-24 14:23:56.000000 clubscore-0.2.3/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1161 2023-06-24 10:52:02.000000 clubscore-0.2.3/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     4241 2023-06-24 13:03:31.000000 clubscore-0.2.3/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.3/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     6333 2023-06-24 14:44:16.000000 clubscore-0.2.3/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.266713 clubscore-0.2.3/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      452 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-06-24 15:34:53.000000 clubscore-0.2.3/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-06-24 15:34:53.275134 clubscore-0.2.3/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-06-24 15:19:52.000000 clubscore-0.2.3/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-24 15:34:53.273607 clubscore-0.2.3/tests/
--rw-r--r--   0 dave       (501) staff       (20)     1966 2023-06-24 14:08:30.000000 clubscore-0.2.3/tests/test_templates.py
--rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-26 23:43:55.308632 clubscore-0.2.4/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.2.4/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-26 23:43:55.308229 clubscore-0.2.4/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.2.4/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-26 23:43:55.298815 clubscore-0.2.4/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)     1206 2023-06-24 15:29:38.000000 clubscore-0.2.4/clubscore/API.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.4/clubscore/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     6412 2023-06-26 23:38:47.000000 clubscore-0.2.4/clubscore/bot.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-26 23:43:55.306031 clubscore-0.2.4/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     5436 2023-06-26 23:27:00.000000 clubscore-0.2.4/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     3148 2023-06-26 23:39:15.000000 clubscore-0.2.4/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1161 2023-06-24 10:52:02.000000 clubscore-0.2.4/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     4241 2023-06-24 13:03:31.000000 clubscore-0.2.4/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.4/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     6339 2023-06-26 23:36:15.000000 clubscore-0.2.4/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-26 23:43:55.302048 clubscore-0.2.4/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-26 23:43:55.000000 clubscore-0.2.4/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      452 2023-06-26 23:43:55.000000 clubscore-0.2.4/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-06-26 23:43:55.000000 clubscore-0.2.4/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-06-26 23:43:55.000000 clubscore-0.2.4/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-06-26 23:43:55.000000 clubscore-0.2.4/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-06-26 23:43:55.308748 clubscore-0.2.4/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-06-26 23:41:11.000000 clubscore-0.2.4/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-26 23:43:55.307502 clubscore-0.2.4/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1966 2023-06-24 14:08:30.000000 clubscore-0.2.4/tests/test_templates.py
+-rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.2.4/tests/test_utils.py
```

### Comparing `clubscore-0.2.3/LICENSE` & `clubscore-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.3/PKG-INFO` & `clubscore-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.2.3/clubscore/API.py` & `clubscore-0.2.4/clubscore/API.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.3/clubscore/bot.py` & `clubscore-0.2.4/clubscore/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import importlib
 import xml.etree.ElementTree as ET
 from io import BytesIO
 import clubscore.utils as u
 import json
 import traceback
 import requests
+from telebot import types
 
 
 def insertAction(bot, message, command):
     d = {}
     d["bot"] = bot
     d["user_id"] = message.from_user.id
     d["name"] = message.from_user.first_name
@@ -36,77 +37,109 @@
 
     with open(single_input) as file:
         comandi_elite = json.load(file)
 
     with open(single_api) as file:
         singleapi = json.load(file)
 
+    reply_markup = None
     print(comandi_elite)
     print(singleapi)
 
+    reply_markup = types.ReplyKeyboardMarkup(row_width=2)
+
+    button = types.InlineKeyboardButton(text="/start")
+    reply_markup.add(button)
+    button = types.InlineKeyboardButton(text="/help")
+    reply_markup.add(button)
+    button = types.InlineKeyboardButton(text="/teams")
+    reply_markup.add(button)
+
+
+    for command_data in singleapi:
+        callback_data = "/" + command_data  # Remove the leading '/'
+        button = types.InlineKeyboardButton(text=callback_data)
+        reply_markup.add(button)
+
+    for command_data in comandi_elite:
+        button_text = f"{command_data}"
+        callback_data = "/" + command_data  # Remove the leading '/'
+        button = types.InlineKeyboardButton(text=callback_data)
+        reply_markup.add(button)
+
     bot = telebot.TeleBot(API_KEY)
 
     def update_status(message):
         d[message.from_user.id] = message.text.replace('/', '')
 
+
     @bot.message_handler(commands=['start'])
-    def start(message):
-        update_status(message)
-        bot.send_message(message.chat.id, f"Welcome in {BOT}! A Clubscore product!")
-        help(message)
+    def send_welcome(message):
+        # Send a welcome message with the command menu
+        bot.send_message(message.chat.id, f"Welcome in {BOT}!🤖\n A Clubscore® product!", reply_markup=reply_markup)
+
 
     @bot.message_handler(commands=['teams'])
     def teams(message):
         bot.send_message(message.chat.id, u.print_file_tree("teams"))
 
     @bot.message_handler(commands=['help'])
     def help(message):
         s = "You have the following commands:\n\n"
+        s += "/start \n \help \n /teams\n"
         for e in sorted(comandi_elite):
             s += "/" + e + "\n"
         for e in sorted(singleapi):
             s += "/" + e + "\n"
         bot.send_message(message.chat.id, s)
 
 
     @bot.message_handler(commands=[k for k in comandi_elite])
     def risultati(message):
         m = message.text.replace('/', '')
         template = comandi_elite[m]
-        print(template)
+        #print(template)
         update_status(message)
         bot.send_message(message.chat.id, u.getTemplateGuide(template))
 
     @bot.message_handler(commands=[k for k in singleapi])
     def risultati(message):
-        m = message.text.replace('/', '')
-        template = singleapi[m]
+        try:
+            m = message.text.replace('/', '')
+            template = singleapi[m]
 
-        function_name = u.getTemplateText(template, "API").strip()
-        params = u.getTemplateText(template, "PARAMETERS").strip().split("\n")
 
-        module_name = "clubscore.API"
-        module = importlib.import_module(module_name)
-        function = getattr(module, function_name)
+            function_name = u.getTemplateText(template, "API").strip()
+            params = u.getTemplateText(template, "PARAMETERS").strip().split("\n")
 
-        lista = function(*params)
+            module_name = "clubscore.API"
+            module = importlib.import_module(module_name)
+            function = getattr(module, function_name)
 
-        root = ET.parse(template).getroot()
-        width = int(root.attrib["width"])
-        height = int(root.attrib["height"])
+            lista = function(*params)
 
-        image = Image.new('RGB', (width, height), color=(255, 255, 255))
-        CONTAINER.interpretaTemplate(image, template, lista)
+            root = ET.parse(template).getroot()
+            width = int(root.attrib["width"])
+            height = int(root.attrib["height"])
 
-        img_io = BytesIO()
-        image.save(img_io, 'PNG', quality=90)
-        img_io.seek(0)
+            image = Image.new('RGB', (width, height), color=(255, 255, 255))
+            CONTAINER.interpretaTemplate(image, template, lista)
+
+            img_io = BytesIO()
+            image.save(img_io, 'PNG', quality=90)
+            img_io.seek(0)
+
+            bot.send_document(message.chat.id, document=img_io, visible_file_name="out.png", reply_markup=reply_markup)
+            insertAction(BOT, message, m)
+
+        except Exception as e:
+            print("An exception occurred")
+            traceback.print_exc()
+            bot.send_message(message.chat.id, "C'è stato un problema, prova a rilanciare il comando")
 
-        bot.send_document(message.chat.id, document=img_io, visible_file_name="out.png")
-        insertAction(BOT, message, m)
 
     # todo rinominare: serve per far funzionare il message handler
     def risultato(message):
         if message.text != '':
             return True
         return False
 
@@ -122,15 +155,15 @@
 
         CONTAINER.interpretaTemplate(image, template, text)
 
         img_io = BytesIO()
         image.save(img_io, 'PNG', quality=90)
         img_io.seek(0)
 
-        bot.send_document(message.chat.id, document=img_io, visible_file_name="out.png")
+        bot.send_document(message.chat.id, document=img_io, visible_file_name="out.png", reply_markup=reply_markup)
 
 
     @bot.message_handler(func=risultato)
     def messaggi(message):
         user = message.from_user.id
         print(message)
```

### Comparing `clubscore-0.2.3/clubscore/objects/CONTAINER.py` & `clubscore-0.2.4/clubscore/objects/CONTAINER.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         return CONTAINER(image, x + int(dict["x"]), y + int(dict["y"]), width, height, elements)
 
 
 
     @staticmethod
     def initiateMultiple(image, root, el, lines, template):
 
+
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
         dict = el.attrib
 
         width = 0 if "width" not in dict else int(dict["width"])
         height = 0 if "height" not in dict else int(dict["height"])
 
@@ -101,18 +102,18 @@
             current_y += int(u.getTemplateAttribute(template,"paddingY")) if u.getTemplateAttribute(template,"paddingY") else padding_y
 
         return CONTAINER(image, x + int(dict["x"]), y + int(dict["y"]), width, height, multiple_elements)
 
 
     @staticmethod
     def interpretaTemplate(image, template, lines):
+
         if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
             template = "../" + template
 
-
         tree = ET.parse(template)
         root = tree.getroot()
         children = list(root)
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
```

### Comparing `clubscore-0.2.3/clubscore/objects/IMG.py` & `clubscore-0.2.4/clubscore/objects/IMG.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         else:
 
             if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
                 dict["foto"] = "../" + dict["foto"]
 
             if "*" in dict["foto"]:
                 testo = lines.pop(0).strip()
-                print(testo)
+                #print(testo)
 
                 if "!" in testo:
                     rgb = (255, 255, 255)
                     testo.replace("!","")
 
                 elif "?" in testo:
                     rgb = (0, 0, 0)
@@ -91,15 +91,14 @@
                     #dovrebbe succedere sempre, tranne quando lancio il test di trasparenza
                     path = dict["foto"].split("/*")[0]
                     testo = u.matchWord(testo, u.getTeams(path))
                     dict["foto"] = f"{path}/{testo}.png"
                 else:
                     dict["foto"] = testo
 
-                print()
 
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
 
 
         centerX = True if "centerX" not in dict or dict["centerX"] is "True" else False
```

### Comparing `clubscore-0.2.3/clubscore/objects/RECTANGLE.py` & `clubscore-0.2.4/clubscore/objects/RECTANGLE.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.3/clubscore/objects/TEXT.py` & `clubscore-0.2.4/clubscore/objects/TEXT.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.3/clubscore/utils.py` & `clubscore-0.2.4/clubscore/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,21 +172,21 @@
 def getTeams(path):
     return [os.path.basename(elem).replace('.png', '') for elem in glob.glob(path + '/*.png')]
 
 def getTeamsFromTXT(path):
     if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
         path = "../" + path
 
-    print(path)
+    #print(path)
 
     if ".txt" in path:
         f = open(path)
         f = f.readlines()
         f = [s.strip() for s in f]
-        print(f)
+        #print(f)
         return f
 
 
 def getTemplateText(template,s):
     if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
         template = "../" + template
 
@@ -206,15 +206,15 @@
     return s
 
 def getTemplateGuide(template):
     return getTemplateText(template,"GUIDA")
 
 
 def getTemplateAttribute(template,attribute):
-    if os.environ['ENV'] == 'testing':
+    if os.environ.get('ENV') == 'testing':
         template = "../" + template
 
     tree = ET.parse(template)
     root = tree.getroot()
     return root.attrib[attribute] if attribute in root.attrib else False
```

### Comparing `clubscore-0.2.3/clubscore.egg-info/PKG-INFO` & `clubscore-0.2.4/clubscore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.2.3/setup.py` & `clubscore-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.2.3',
+    version='0.2.4',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

### Comparing `clubscore-0.2.3/tests/test_templates.py` & `clubscore-0.2.4/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.3/tests/test_utils.py` & `clubscore-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

