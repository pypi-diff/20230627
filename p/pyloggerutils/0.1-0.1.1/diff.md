# Comparing `tmp/pyloggerutils-0.1.tar.gz` & `tmp/pyloggerutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggerutils-0.1.tar", last modified: Tue Jun 27 13:36:47 2023, max compression
+gzip compressed data, was "pyloggerutils-0.1.1.tar", last modified: Tue Jun 27 13:43:57 2023, max compression
```

## Comparing `pyloggerutils-0.1.tar` & `pyloggerutils-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:36:47.790827 pyloggerutils-0.1/
--rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1/LICENSE
--rw-rw-rw-   0        0        0      748 2023-06-27 13:36:47.791829 pyloggerutils-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 13:36:47.778313 pyloggerutils-0.1/pyloggerutils/
--rw-rw-rw-   0        0        0     1082 2023-06-27 11:45:43.000000 pyloggerutils-0.1/pyloggerutils/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-27 12:05:34.000000 pyloggerutils-0.1/pyloggerutils/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:36:47.790827 pyloggerutils-0.1/pyloggerutils.egg-info/
--rw-rw-rw-   0        0        0      748 2023-06-27 13:36:47.000000 pyloggerutils-0.1/pyloggerutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-27 13:36:47.000000 pyloggerutils-0.1/pyloggerutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:36:47.000000 pyloggerutils-0.1/pyloggerutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 13:36:47.000000 pyloggerutils-0.1/pyloggerutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 13:36:47.791829 pyloggerutils-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1588 2023-06-27 13:36:46.000000 pyloggerutils-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:43:57.175093 pyloggerutils-0.1.1/
+-rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      757 2023-06-27 13:43:57.175093 pyloggerutils-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 13:43:57.166093 pyloggerutils-0.1.1/pyloggerutils/
+-rw-rw-rw-   0        0        0     1082 2023-06-27 13:39:27.000000 pyloggerutils-0.1.1/pyloggerutils/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-27 12:05:34.000000 pyloggerutils-0.1.1/pyloggerutils/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:43:57.174093 pyloggerutils-0.1.1/pyloggerutils.egg-info/
+-rw-rw-rw-   0        0        0      757 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 13:43:57.176092 pyloggerutils-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2023-06-27 13:43:54.000000 pyloggerutils-0.1.1/setup.py
```

### Comparing `pyloggerutils-0.1/LICENSE` & `pyloggerutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1/PKG-INFO` & `pyloggerutils-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyloggerutils
-Version: 0.1
+Version: 0.1.1
 Summary: This is Python Logger
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/PyLogger/archive/refs/tags/v-0.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Logger,Easy,PySy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyloggerutils-0.1/pyloggerutils/__init__.py` & `pyloggerutils-0.1.1/pyloggerutils/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .logger import Logger as Logger
 LOG_LEVELS = {
     "DEBUG": 1,
     "INFO": 2,
     "WARNING": 3,
     "CRITICAL": 4,
     "ERROR": 5
 }
@@ -31,8 +30,9 @@
     },
     "formatters":{
         "std_out": {
             "format": "%(asctime)s : %(levelname)s : %(module)s : %(funcName)s : %(lineno)d : (Process Details : (%(process)d, %(processName)s), Thread Details : (%(thread)d, %(threadName)s))\nLog : %(message)s",
             "datefmt":"%d-%m-%Y %I:%M:%S"
         }
     }
-}
+}
+from .logger import Logger as Logger
```

### Comparing `pyloggerutils-0.1/pyloggerutils/logger.py` & `pyloggerutils-0.1.1/pyloggerutils/logger.py`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1/pyloggerutils.egg-info/PKG-INFO` & `pyloggerutils-0.1.1/pyloggerutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyloggerutils
-Version: 0.1
+Version: 0.1.1
 Summary: This is Python Logger
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/PyLogger/archive/refs/tags/v-0.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Logger,Easy,PySy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyloggerutils-0.1/setup.py` & `pyloggerutils-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'pyloggerutils',         # How you named your package folder (MyLib)
   packages = ['pyloggerutils'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = """This is Python Logger""",   # Give a short description about your library
   author = 'Sabari Rajan',                   # Type in your name
   author_email = 'mailme@isbarirajan.com',      # Type in your E-Mail
   url = 'https://github.com/ISabariRajan',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ISabariRajan/PyLogger/archive/refs/tags/v-0.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz',    # I explain this later on
   keywords = ['Logger', 'Easy', 'PySy'],   # Keywords that define your package best
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

