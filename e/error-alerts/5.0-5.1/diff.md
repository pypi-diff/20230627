# Comparing `tmp/error-alerts-5.0.tar.gz` & `tmp/error-alerts-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-5.0.tar", last modified: Tue Jun 27 12:20:49 2023, max compression
+gzip compressed data, was "error-alerts-5.1.tar", last modified: Tue Jun 27 12:24:15 2023, max compression
```

## Comparing `error-alerts-5.0.tar` & `error-alerts-5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:20:49.459128 error-alerts-5.0/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.0/.gitignore
--rw-rw-rw-   0        0        0     1301 2023-06-27 12:20:49.459128 error-alerts-5.0/PKG-INFO
--rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:20:49.454131 error-alerts-5.0/error_alerts/
--rw-rw-rw-   0        0        0     3283 2023-06-27 12:16:26.000000 error-alerts-5.0/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:20:49.458129 error-alerts-5.0/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-06-27 12:20:49.000000 error-alerts-5.0/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-27 12:20:49.000000 error-alerts-5.0/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:20:49.000000 error-alerts-5.0/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 12:20:49.000000 error-alerts-5.0/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 12:20:49.000000 error-alerts-5.0/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 12:20:49.460127 error-alerts-5.0/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-27 12:20:46.000000 error-alerts-5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:24:15.910360 error-alerts-5.1/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.1/.gitignore
+-rw-rw-rw-   0        0        0     1301 2023-06-27 12:24:15.910360 error-alerts-5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:24:15.904364 error-alerts-5.1/error_alerts/
+-rw-rw-rw-   0        0        0     3307 2023-06-27 12:24:07.000000 error-alerts-5.1/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:24:15.909361 error-alerts-5.1/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 12:24:15.911360 error-alerts-5.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-27 12:24:11.000000 error-alerts-5.1/setup.py
```

### Comparing `error-alerts-5.0/PKG-INFO` & `error-alerts-5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.0
+Version: 5.1
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-5.0/README.md` & `error-alerts-5.1/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-5.0/error_alerts/__init__.py` & `error-alerts-5.1/error_alerts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     'The service is currently unavailable', # Google sheets API down
     'Could not authenticate you', # Twitter app suspended
     ]
 
 class alerts(Bot):
     def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
         if token:
-            super().__init__(token=token)
-            # self.message = bot.send_message
-            # self._bot = bot
+            bot = super()
+            bot.__init__(token=token)
+            self.message = bot.send_message
+            self.telegram_bot = bot
 
         self.channel = channel
         if logger:
             self.log, self.current_time = logger.log, logger.current_time
         else:
             self.log = None
         self.full_error = full_error
@@ -81,8 +82,8 @@
             else:
                 self.log(*items, level=level)
             self.log(level=level)
         elif level != 'debug': # Don't print debug only messages
             print(*items)
             print()
 
-# telegram = alerts
+telegram = alerts
```

### Comparing `error-alerts-5.0/error_alerts.egg-info/PKG-INFO` & `error-alerts-5.1/error_alerts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.0
+Version: 5.1
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

