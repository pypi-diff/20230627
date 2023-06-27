# Comparing `tmp/polylog-0.0.1.tar.gz` & `tmp/polylog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylog-0.0.1.tar", last modified: Wed Jun  7 23:18:52 2023, max compression
+gzip compressed data, was "polylog-0.0.2.tar", last modified: Tue Jun 27 17:16:30 2023, max compression
```

## Comparing `polylog-0.0.1.tar` & `polylog-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 23:18:52.422814 polylog-0.0.1/
--rw-r--r--   0 tom       (1000) tom       (1000)     2340 2023-06-07 23:18:52.422814 polylog-0.0.1/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1210 2023-06-07 23:17:00.000000 polylog-0.0.1/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 23:18:52.422814 polylog-0.0.1/polylog/
--rw-r--r--   0 tom       (1000) tom       (1000)       33 2023-06-07 19:50:18.000000 polylog-0.0.1/polylog/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2878 2023-06-07 18:40:16.000000 polylog-0.0.1/polylog/logger.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 23:18:52.422814 polylog-0.0.1/polylog.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2340 2023-06-07 23:18:52.000000 polylog-0.0.1/polylog.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      225 2023-06-07 23:18:52.000000 polylog-0.0.1/polylog.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-07 23:18:52.000000 polylog-0.0.1/polylog.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-06-07 23:18:52.000000 polylog-0.0.1/polylog.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       13 2023-06-07 23:18:52.000000 polylog-0.0.1/polylog.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)     2276 2023-06-07 23:12:23.000000 polylog-0.0.1/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-07 23:18:52.422814 polylog-0.0.1/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      704 2023-06-07 23:12:44.000000 polylog-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:30.607716 polylog-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-27 17:16:30.607716 polylog-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-27 17:16:13.000000 polylog-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:30.603716 polylog-0.0.2/polylog/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 17:16:13.000000 polylog-0.0.2/polylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 17:16:13.000000 polylog-0.0.2/polylog/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:30.607716 polylog-0.0.2/polylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-27 17:16:21.000000 polylog-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:16:30.607716 polylog-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-27 17:16:13.000000 polylog-0.0.2/setup.py
```

### Comparing `polylog-0.0.1/PKG-INFO` & `polylog-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.0.1
+Version: 0.0.2
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.0.1/README.md` & `polylog-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `polylog-0.0.1/polylog/logger.py` & `polylog-0.0.2/polylog/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import logging
 import logging.handlers
 import threading
 from contextvars import ContextVar
 
 # Define context variables for traceId and spanId
-trace_id_var = ContextVar('trace_id', default=None)
-span_id_var = ContextVar('span_id', default=None)
+trace_id_var = ContextVar("trace_id", default=None)
+span_id_var = ContextVar("span_id", default=None)
+
 
 class CustomFormatter(logging.Formatter):
     LEVEL_COLORS = [
         (logging.DEBUG, "\x1b[40;1m"),
         (logging.INFO, "\x1b[34;1m"),
         (logging.WARNING, "\x1b[33;1m"),
         (logging.ERROR, "\x1b[31m"),
@@ -29,54 +30,62 @@
         if formatter is None:
             formatter = self.FORMATS[logging.DEBUG]
 
         # Override the traceback to always print in red
         if record.exc_info:
             text = formatter.formatException(record.exc_info)
             record.exc_text = f"\x1b[31m{text}\x1b[0m"
-        
+
         # Adding context data to record
         record.traceId = trace_id_var.get()
         record.spanId = span_id_var.get()
 
         output = formatter.format(record)
         # Remove the cache layer
         record.exc_text = None
         return output
 
+
 # Define a lock for logger switching
 logger_lock = threading.Lock()
 
 def setup_logger(module_name: str) -> logging.Logger:
     with logger_lock:
         # create logger
         library, _, _ = module_name.partition(".py")
         logger = logging.getLogger(library)
-        logger.setLevel(logging.INFO)
 
-        log_level = "INFO"
+        log_level = os.getenv("LOG_LEVEL", "INFO")
         level = logging.getLevelName(log_level.upper())
+        logger.setLevel(level)
 
         # create console handler
         console_handler = logging.StreamHandler()
         console_handler.setLevel(level)
         console_handler.setFormatter(CustomFormatter())
         # Add console handler to logger
         logger.addHandler(console_handler)
 
         if os.getenv("LOGGING") == "True":  # Check if logging is enabled
             # specify that the log file path is the same as `main.py` file path
             grandparent_dir = os.path.abspath(f"{__file__}/../../")
-            log_name = "logger.log"
+            log_name = os.getenv("LOG_FILE_NAME", "logger.log")
             log_path = os.path.join(grandparent_dir, log_name)
             # create local log handler
-            log_handler = logging.handlers.RotatingFileHandler(
-                filename=log_path,
-                encoding="utf-8",
-                maxBytes=32 * 1024 * 1024,  # 32 MiB
-                backupCount=2,  # Rotate through 5 files
-            )
-            log_handler.setFormatter(CustomFormatter())
-            log_handler.setLevel(level)
-            logger.addHandler(log_handler)
+            try:
+                log_handler = logging.handlers.RotatingFileHandler(
+                    filename=log_path,
+                    encoding="utf-8",
+                    maxBytes=int(
+                        os.getenv("LOG_MAX_BYTES", 32 * 1024 * 1024)
+                    ),  # 32 MiB
+                    backupCount=int(
+                        os.getenv("LOG_BACKUP_COUNT", 2)
+                    ),  # Rotate through 2 files
+                )
+                log_handler.setFormatter(CustomFormatter())
+                log_handler.setLevel(level)
+                logger.addHandler(log_handler)
+            except Exception as e:
+                logger.error(f"Failed to create file handler: {e}")
 
         return logger
```

### Comparing `polylog-0.0.1/polylog.egg-info/PKG-INFO` & `polylog-0.0.2/polylog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.0.1
+Version: 0.0.2
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.0.1/pyproject.toml` & `polylog-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "polylog"  # Required
-version = "0.0.1"  # Required
+version = "0.0.2"
 description = "A custom python logging package"  # Optional
 
 readme = "README.md" # Optional
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 keywords = []  # Optional
```

### Comparing `polylog-0.0.1/setup.py` & `polylog-0.0.2/setup.py`

 * *Files identical despite different names*

