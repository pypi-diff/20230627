# Comparing `tmp/error-alerts-4.5.tar.gz` & `tmp/error-alerts-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.5.tar", last modified: Sun Jun 25 18:03:45 2023, max compression
+gzip compressed data, was "error-alerts-4.6.tar", last modified: Tue Jun 27 11:16:18 2023, max compression
```

## Comparing `error-alerts-4.5.tar` & `error-alerts-4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:03:45.556074 error-alerts-4.5/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.5/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-06-25 18:03:45.556074 error-alerts-4.5/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 18:03:45.551078 error-alerts-4.5/error_alerts/
--rw-rw-rw-   0        0        0     2991 2023-06-25 18:03:36.000000 error-alerts-4.5/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:03:45.555075 error-alerts-4.5/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-06-25 18:03:45.000000 error-alerts-4.5/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-25 18:03:45.000000 error-alerts-4.5/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:03:45.000000 error-alerts-4.5/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 18:03:45.000000 error-alerts-4.5/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-25 18:03:45.000000 error-alerts-4.5/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-25 18:03:45.556074 error-alerts-4.5/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-25 18:03:42.000000 error-alerts-4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:16:18.536996 error-alerts-4.6/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.6/.gitignore
+-rw-rw-rw-   0        0        0     1305 2023-06-27 11:16:18.537994 error-alerts-4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:16:18.532998 error-alerts-4.6/error_alerts/
+-rw-rw-rw-   0        0        0     3116 2023-06-27 11:16:13.000000 error-alerts-4.6/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:16:18.536996 error-alerts-4.6/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 11:16:18.537994 error-alerts-4.6/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-27 11:16:10.000000 error-alerts-4.6/setup.py
```

### Comparing `error-alerts-4.5/PKG-INFO` & `error-alerts-4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.5
+Version: 4.6
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-4.5/README.md` & `error-alerts-4.6/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-4.5/error_alerts/__init__.py` & `error-alerts-4.6/error_alerts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import traceback
 from telegram import Bot, InlineKeyboardButton, InlineKeyboardMarkup
 
-class telegram:
+DEFAULT_IGNORED_ERRORS = [
+    'The service is currently unavailable', # Google sheets API down
+    'Could not authenticate you', # Twitter app suspended
+    ]
+
+class telegram(Bot):
     def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
         if token:
-            self.bot = Bot(token=token)
-            self.username = self.bot.username
+            super().__init__(token=token)
+
         self.channel = channel
         self.logger = logger
         self.full_error = full_error
         self.raise_error = raise_error
         self.resend_repeat_errors = resend_repeat_errors
         self.last_error = None
+
     def send(self, title='Error', exception=None, channel=None):
         if not channel:
             channel = self.channel
         if self.full_error:
             error = traceback.format_exc()
         else:
             error = str(exception)
         message = f'{title}: {error}'
-        if error == self.last_error and not self.resend_repeat_errors:
-            self.printer(message, level='error')
+        
+        self.printer(message, level='error')
+
         if error != self.last_error or self.resend_repeat_errors:
-            self.printer(message, level='error')
+
             if channel:
-                try:
-                    self.bot.send_message(channel, message[:4096])
-                except Exception as telegram_error:
-                    self.printer('Error sending alert message to Telegram:', telegram_error, level='error')
-            self.last_error = error
+                if all(ignored_error not in error for ignored_error in DEFAULT_IGNORED_ERRORS):
+                    self.last_error = error
+
+                    try:
+                        self.send_message(channel, message[:4096])
+                    except Exception as telegram_error:
+                        self.printer('Error sending alert message to Telegram:', telegram_error, level='error')
+
         if self.raise_error:
             raise Exception('Raiser') from exception
 
     def send_message(self, *messages, print_message=True, current_time=True, channel=None, buttons_dict={}):
         if not channel:
             channel = self.channel
         final_message = ''
@@ -41,15 +51,15 @@
             final_message += message
             final_message += ' '
         if print_message:
             self.printer(final_message, current_time=current_time)
         if channel:
             buttons_markup = self.convert_dict_to_buttons(buttons_dict)
             try:
-                message = self.bot.send_message(channel, final_message[:4096], reply_markup=buttons_markup)
+                message = self.send_message(channel, final_message[:4096], reply_markup=buttons_markup)
                 return message
             except Exception as telegram_error:
                 self.printer('Error sending message to Telegram:', telegram_error, level='error')
         return None
 
     def convert_dict_to_buttons(self, buttons_dict):
         buttons = []
```

### Comparing `error-alerts-4.5/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.6/error_alerts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.5
+Version: 4.6
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

