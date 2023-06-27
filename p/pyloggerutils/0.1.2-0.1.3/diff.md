# Comparing `tmp/pyloggerutils-0.1.2.tar.gz` & `tmp/pyloggerutils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggerutils-0.1.2.tar", last modified: Tue Jun 27 14:02:09 2023, max compression
+gzip compressed data, was "pyloggerutils-0.1.3.tar", last modified: Tue Jun 27 18:17:32 2023, max compression
```

## Comparing `pyloggerutils-0.1.2.tar` & `pyloggerutils-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 14:02:09.948789 pyloggerutils-0.1.2/
--rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1029 2023-06-27 14:02:09.948789 pyloggerutils-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 14:02:09.920474 pyloggerutils-0.1.2/pyloggerutils/
--rw-rw-rw-   0        0        0     1082 2023-06-27 13:39:27.000000 pyloggerutils-0.1.2/pyloggerutils/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-27 12:05:34.000000 pyloggerutils-0.1.2/pyloggerutils/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:02:09.947791 pyloggerutils-0.1.2/pyloggerutils.egg-info/
--rw-rw-rw-   0        0        0     1029 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 14:02:09.949791 pyloggerutils-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1850 2023-06-27 13:59:03.000000 pyloggerutils-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:17:32.828725 pyloggerutils-0.1.3/
+-rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1029 2023-06-27 18:17:32.828725 pyloggerutils-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 18:17:32.814725 pyloggerutils-0.1.3/pyloggerutils/
+-rw-rw-rw-   0        0        0     1397 2023-06-27 18:09:21.000000 pyloggerutils-0.1.3/pyloggerutils/__init__.py
+-rw-rw-rw-   0        0        0     2396 2023-06-27 18:10:34.000000 pyloggerutils-0.1.3/pyloggerutils/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:17:32.827724 pyloggerutils-0.1.3/pyloggerutils.egg-info/
+-rw-rw-rw-   0        0        0     1029 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 18:17:32.833745 pyloggerutils-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-27 18:16:28.000000 pyloggerutils-0.1.3/setup.py
```

### Comparing `pyloggerutils-0.1.2/LICENSE` & `pyloggerutils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1.2/PKG-INFO` & `pyloggerutils-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyloggerutils
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is Python Logger
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.3.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Logger,Easy,PySy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyloggerutils-0.1.2/pyloggerutils/__init__.py` & `pyloggerutils-0.1.3/pyloggerutils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,47 @@
+LOG_DATE_FORMAT = "%d-%m-%Y %I:%M:%S"
+LOG_FORMAT_LIMITERS = {
+    "MODULE": 40
+}
 LOG_LEVELS = {
     "DEBUG": 1,
     "INFO": 2,
     "WARNING": 3,
     "CRITICAL": 4,
     "ERROR": 5
 }
 
 LOG_CONFIG = {
     "version": 1,
     "root": {
         "handlers": ["console", "fileHandler", "fileErrorHandler"],
+        "level": "NOTSET"
     },
     "handlers":{
         "console":{
             "formatter": "std_out",
             "class": "logging.StreamHandler",
             "level": "DEBUG"
         },
-        "console":{
+        "fileHandler":{
             "formatter": "std_out",
-            "class": "handlers.TimedRotatingFileHandler",
-            "level": "DEBUG"
+            "class": "logging.handlers.TimedRotatingFileHandler",
+            "level": "DEBUG",
+            "filename": "testing.log"
+            # "args": ('testing.log','w0',0,5)
         },
-        "console":{
+        "fileErrorHandler":{
             "formatter": "std_out",
-            "class": "handlers.TimedRotatingFileHandler",
-            "level": "ERROR"
+            "class": "logging.handlers.TimedRotatingFileHandler",
+            "level": "ERROR",
+            "filename": "testing-error.log"
         }
     },
     "formatters":{
         "std_out": {
-            "format": "%(asctime)s : %(levelname)s : %(module)s : %(funcName)s : %(lineno)d : (Process Details : (%(process)d, %(processName)s), Thread Details : (%(thread)d, %(threadName)s))\nLog : %(message)s",
+            # "format": "%(asctime)s : %(levelname)s : %(module)s : %(funcName)s : %(lineno)d : (Process Details : (%(process)d, %(processName)s), Thread Details : (%(thread)d, %(threadName)s))\nLog : %(message)s",
+            "format": "%(message)s",
             "datefmt":"%d-%m-%Y %I:%M:%S"
         }
     }
 }
 from .logger import Logger as Logger
```

### Comparing `pyloggerutils-0.1.2/pyloggerutils.egg-info/PKG-INFO` & `pyloggerutils-0.1.3/pyloggerutils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyloggerutils
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is Python Logger
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.3.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Logger,Easy,PySy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyloggerutils-0.1.2/setup.py` & `pyloggerutils-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'pyloggerutils',         # How you named your package folder (MyLib)
   packages = ['pyloggerutils'],   # Chose the same as "name"
-  version = '0.1.2',      # Start with a small number and increase it with every change you make
+  version = '0.1.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = """This is Python Logger""",   # Give a short description about your library
   author = 'Sabari Rajan',                   # Type in your name
   author_email = 'mailme@isbarirajan.com',      # Type in your E-Mail
   url = 'https://github.com/ISabariRajan',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.3.tar.gz',    # I explain this later on
   keywords = ['Logger', 'Easy', 'PySy'],   # Keywords that define your package best
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

