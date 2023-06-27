# Comparing `tmp/error-alerts-4.8.tar.gz` & `tmp/error-alerts-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.8.tar", last modified: Tue Jun 27 12:00:04 2023, max compression
+gzip compressed data, was "error-alerts-4.9.tar", last modified: Tue Jun 27 12:03:06 2023, max compression
```

## Comparing `error-alerts-4.8.tar` & `error-alerts-4.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:00:04.328118 error-alerts-4.8/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.8/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-06-27 12:00:04.328118 error-alerts-4.8/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:00:04.321123 error-alerts-4.8/error_alerts/
--rw-rw-rw-   0        0        0     3491 2023-06-27 11:59:58.000000 error-alerts-4.8/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:00:04.327119 error-alerts-4.8/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-06-27 12:00:03.000000 error-alerts-4.8/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-27 12:00:04.000000 error-alerts-4.8/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:00:03.000000 error-alerts-4.8/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 12:00:03.000000 error-alerts-4.8/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 12:00:03.000000 error-alerts-4.8/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 12:00:04.329117 error-alerts-4.8/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-27 12:00:01.000000 error-alerts-4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:03:06.491555 error-alerts-4.9/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.9/.gitignore
+-rw-rw-rw-   0        0        0     1301 2023-06-27 12:03:06.491555 error-alerts-4.9/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:03:06.486559 error-alerts-4.9/error_alerts/
+-rw-rw-rw-   0        0        0     3509 2023-06-27 12:02:58.000000 error-alerts-4.9/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:03:06.490556 error-alerts-4.9/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-06-27 12:03:06.000000 error-alerts-4.9/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-27 12:03:06.000000 error-alerts-4.9/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:03:06.000000 error-alerts-4.9/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 12:03:06.000000 error-alerts-4.9/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 12:03:06.000000 error-alerts-4.9/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 12:03:06.492555 error-alerts-4.9/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-27 12:03:03.000000 error-alerts-4.9/setup.py
```

### Comparing `error-alerts-4.8/PKG-INFO` & `error-alerts-4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.8
+Version: 4.9
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
@@ -20,17 +20,17 @@
 
 `full_error`: Send full traceback with line of code where error occurred (False by default and shown in sample below).
 
 `raise_error`: Raise error and exit code when there is an error. If this is not set to True an alert will be sent and the code will continue running (False by default).
 
 Usage:
 ```
-from error_alerts import telegram
+from error_alerts import alerts
 
-alerts = telegram(token='TELEGRAM_TOKEN', channel=TELEGRAM_CHANNEL_ID, full_error=True, raise_error=True)
+alerts = alerts(token='TELEGRAM_TOKEN', channel=TELEGRAM_CHANNEL_ID, full_error=True, raise_error=True)
 
 try:
     1 / 0
 except Exception as error:
     alerts.send(title='Test', exception=error)
 ```
```

### Comparing `error-alerts-4.8/README.md` & `error-alerts-4.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 `full_error`: Send full traceback with line of code where error occurred (False by default and shown in sample below).
 
 `raise_error`: Raise error and exit code when there is an error. If this is not set to True an alert will be sent and the code will continue running (False by default).
 
 Usage:
 ```
-from error_alerts import telegram
+from error_alerts import alerts
 
-alerts = telegram(token='TELEGRAM_TOKEN', channel=TELEGRAM_CHANNEL_ID, full_error=True, raise_error=True)
+alerts = alerts(token='TELEGRAM_TOKEN', channel=TELEGRAM_CHANNEL_ID, full_error=True, raise_error=True)
 
 try:
     1 / 0
 except Exception as error:
     alerts.send(title='Test', exception=error)
 ```
```

### Comparing `error-alerts-4.8/error_alerts/__init__.py` & `error-alerts-4.9/error_alerts/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     'The service is currently unavailable', # Google sheets API down
     'Could not authenticate you', # Twitter app suspended
     ]
 
 class alerts(Bot):
     def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
         if token:
-            self.bot = super()
-            self.bot.__init__(token=token)
+            bot = super()
+            bot.__init__(token=token)
             self.message = bot.send_message
+            self._bot = bot
 
         self.channel = channel
         if logger:
             self.log, self.current_time = logger.log, logger.current_time
         else:
             self.log = None
         self.full_error = full_error
```

### Comparing `error-alerts-4.8/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.9/error_alerts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.8
+Version: 4.9
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
@@ -20,17 +20,17 @@
 
 `full_error`: Send full traceback with line of code where error occurred (False by default and shown in sample below).
 
 `raise_error`: Raise error and exit code when there is an error. If this is not set to True an alert will be sent and the code will continue running (False by default).
 
 Usage:
 ```
-from error_alerts import telegram
+from error_alerts import alerts
 
-alerts = telegram(token='TELEGRAM_TOKEN', channel=TELEGRAM_CHANNEL_ID, full_error=True, raise_error=True)
+alerts = alerts(token='TELEGRAM_TOKEN', channel=TELEGRAM_CHANNEL_ID, full_error=True, raise_error=True)
 
 try:
     1 / 0
 except Exception as error:
     alerts.send(title='Test', exception=error)
 ```
```

