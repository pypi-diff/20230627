# Comparing `tmp/conflog-1.3.0.tar.gz` & `tmp/conflog-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflog-1.3.0.tar", last modified: Wed Jun 14 09:39:16 2023, max compression
+gzip compressed data, was "conflog-1.4.0.tar", last modified: Tue Jun 27 12:51:20 2023, max compression
```

## Comparing `conflog-1.3.0.tar` & `conflog-1.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-14 09:38:36.000000 conflog-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 09:39:16.901686 conflog-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-14 09:38:36.000000 conflog-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.897686 conflog-1.3.0/conflog/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.897686 conflog-1.3.0/conflog/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/handlers/stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/conflog/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/yaml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.897686 conflog-1.3.0/conflog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:39:16.901686 conflog-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 09:38:36.000000 conflog-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/handlers/test_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/handlers/test_stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/test_conflog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-27 12:50:25.000000 conflog-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-27 12:51:20.878944 conflog-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-27 12:50:25.000000 conflog-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.874943 conflog-1.4.0/conflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/conflog/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/handlers/stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/conflog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/yaml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.874943 conflog-1.4.0/conflog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:51:20.878944 conflog-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-27 12:50:25.000000 conflog-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/handlers/test_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/handlers/test_stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/test_conflog.py
```

### Comparing `conflog-1.3.0/LICENSE` & `conflog-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/PKG-INFO` & `conflog-1.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: conflog
-Version: 1.3.0
-Summary: Python logging setup via environment variables and configuration files
-Home-page: https://github.com/cliffano/pyconflog
-Author: Cliffano Subagio
-Author-email: cliffano@gmail.com
-Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
 [![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
 [![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
@@ -46,25 +31,59 @@
       env: "dev"
       id: "123"
  
 And then use it in your Python code:
 
     from conflog import Conflog
 
-    cfl = conflog.Conflog(conf_files=['conflog.yaml'])
+    cfl = Conflog(conf_files=['conflog.yaml'])
     logger = cfl.get_logger('somename')
     logger.debug('Some debug message')
     logger.info('Some info message')
     logger.critical('Some critical message')
 
 It will write the log messages to stdout and file `conflog.log`:
 
     [SOMEAPP] [dev-123] 2023-06-07 10:49:01 INFO Some info message
     [SOMEAPP] [dev-123] 2023-06-07 10:49:52 CRITICAL Some critical message
 
+If you specify environment variables configuration, it will overwrite the configuration files:
+
+    import os
+    from conflog import Conflog
+
+    os.environ['CONFLOG_FORMAT'] = '[ENVAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s'
+    cfl = Conflog(conf_files=['conflog.yaml'])
+    logger.debug('Some debug message')
+    logger.info('Some info message')
+    logger.critical('Some critical message')
+
+It will write the log messages using the format from `CONFLOG_FORMAT` environment variable:
+
+    [ENVAPP] [dev-123] 2023-06-07 10:49:01 INFO Some info message
+    [ENVAPP] [dev-123] 2023-06-07 10:49:52 CRITICAL Some critical message
+
+And if you specify configuration dictionary, it will overwrite everything else:
+
+    import os
+    from conflog import Conflog
+
+    os.environ['CONFLOG_FORMAT'] = '[ENVAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s'
+    cfl = Conflog(
+        conf_files=['conflog.yaml'],
+        conf_dict={'format': '[DICTAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s'})
+    logger.debug('Some debug message')
+    logger.info('Some info message')
+    logger.critical('Some critical message')
+
+It will write the log messages using the format from configuration dictionary:
+
+    [DICTAPP] [dev-123] 2023-06-07 10:49:01 INFO Some info message
+    [DICTAPP] [dev-123] 2023-06-07 10:49:52 CRITICAL Some critical message
+
 Configuration
 -------------
 
 Configuration properties:
 
 | Property | Description | Default | Example |
 | -------- | ----------- | ------- | ------- |
@@ -72,15 +91,17 @@
 | datefmt | Date format | `%d-%b-%y %H:%M:%S` | `%Y-%m-%d %H:%M:%S` |
 | filename | Log file name | `conflog.log` | `someconflog.log` |
 | filemode | Log file mode | `w` | `w` |
 | format | Log message format | %(asctime)s --> %(name)s - %(levelname)s - %(message)s | `[SOMEAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s` |
 | level | Log level, supported values are `debug`, `info`, `warning`, `error`, `critical` | `info` | `critical` |
 | extras | Extra fields to be added to log message. It can be comma separated key value pairs with equal separator, or a key value pairs map for JSON and YAML configuration files | None | `env=dev,id=123` |
 
-Configuration files can be in YAML, JSON, XML, or INI format. Multiple files can be specified in the `conf_files` parameter when initialising `Conflog`, the configuration will be merged in the order of the files, the latter file will override the former file, and environment variables override configuration files' properties.
+Configuration files can be in YAML, JSON, XML, or INI format. Multiple files can be specified in the `conf_files` parameter when initialising `Conflog`, the configuration will be merged in the order of the files, the latter file will overwrites the former file.
+
+Environment variables configuration overwrites configuration files' properties. And finally, configuration dictionary overwrite everything else.
 
 ### YAML
 
 Example YAML configuration file:
 
     ---
     handlers: "stream,file"
@@ -149,15 +170,15 @@
     CONFLOG_FORMAT="[SOMEAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s"
     CONFLOG_LEVEL="info"
     CONFLOG_EXTRAS="env=dev,id=123"
 
 Colophon
 --------
 
-[Developer's Guide](https://cliffano.github.io/developers_guide.html#nodejs)
+[Developer's Guide](https://cliffano.github.io/developers_guide.html#python)
 
 Build reports:
 
 * [Lint report](https://cliffano.github.io/pyconflog/lint/pylint/index.html)
 * [Code complexity report](https://cliffano.github.io/pyconflog/complexity/wily/index.html)
 * [Unit tests report](https://cliffano.github.io/pyconflog/test/pytest/index.html)
 * [Test coverage report](https://cliffano.github.io/pyconflog/coverage/coverage/index.html)
```

### Comparing `conflog-1.3.0/conflog/config.py` & `conflog-1.4.0/conflog/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A module for managing logging configurations.
 """
+from typing import Union
 import logging
 from .loaders import environ_loader, ini_loader, json_loader, xml_loader, yaml_loader
 
 LEVELS = {
     'debug': logging.DEBUG,
     'warning': logging.WARNING,
     'info': logging.INFO,
@@ -19,18 +20,19 @@
 DEFAULT_LEVEL = 'info'
 DEFAULT_EXTRAS = {}
 
 class Config():
     """A class for managing logging configurations.
     """
 
-    def __init__(self, conf_files=None):
+    def __init__(self, conf_files: Union[None, list]=None, conf_dict: Union[None, list]=None):
         """Initialise config by loading and merging
         the configuration options from files and environment
-        variables.
+        variables, with optional configuration dictionary overwriting
+        everything being specified.
         """
 
         self.conf = {}
 
         # Load configurations from files
         for conf_file in (conf_files or []):
 
@@ -44,58 +46,64 @@
                 curr_conf = xml_loader.load(conf_file)
             elif conf_file.endswith('.yaml'):
                 curr_conf = yaml_loader.load(conf_file)
 
             self.conf = {**self.conf, **curr_conf}
 
         # Load configurations from environment variables
+        # Environment variables configuration overwrites all configuration
+        # files supplied
         self.conf = {**self.conf, **environ_loader.load()}
 
-    def get_handlers(self):
+        # Overwrite everything if configuration dictionary is supplied
+        if conf_dict:
+            self.conf = {**self.conf, **conf_dict}
+
+    def get_handlers(self) -> str:
         """Get handlers.
         Handlers is a comma separated value of the handler
         types to be used.
         If handlers is not specified, default to 'stream'.
         Currently supported handlers are 'stream' and 'file'.
         """
         return self.conf.get('handlers', DEFAULT_HANDLERS).split(',')
 
-    def get_datefmt(self):
+    def get_datefmt(self) -> str:
         """Get date format.
         If date format is not specified, default to '%d-%b-%y %H:%M:%S'.
         """
         return self.conf.get('datefmt', DEFAULT_DATEFMT)
 
-    def get_filename(self):
+    def get_filename(self) -> str:
         """Get log filename.
         If log filename is not specified, default to 'conflog.log'.
         """
         return self.conf.get('filename', DEFAULT_FILENAME)
 
-    def get_filemode(self):
+    def get_filemode(self) -> str:
         """Get file mode.
         If file mode is not specified, default to 'w'.
         """
         return self.conf.get('filemode', DEFAULT_FILEMODE)
 
-    def get_format(self):
+    def get_format(self) -> str:
         """Get log format.
         If log format is not specified, default to
         '%(asctime)s --> %(name)s - %(levelname)s - %(message)s'.
         """
         return self.conf.get('format', DEFAULT_FORMAT)
 
-    def get_level(self):
+    def get_level(self) -> int:
         """Get log level.
         If log level is not specified, default to 'info'.
         """
         level = self.conf.get('level', DEFAULT_LEVEL)
         return LEVELS[level]
 
-    def get_extras(self):
+    def get_extras(self) -> dict:
         """Get extras.
         Extras is a dictionary of extra message parameters
         to be added to the log.
         If extras is not specified, default to an empty dictionary.
         """
         extras = self.conf.get('extras', DEFAULT_EXTRAS)
         if isinstance(extras, str):
```

### Comparing `conflog-1.3.0/conflog/loaders/ini_loader.py` & `conflog-1.4.0/conflog/loaders/ini_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """INI configuration loader.
 """
 import configparser
 import io
 from . import PARAMS
 
-def load(conf_file):
+def load(conf_file: str) -> dict:
     """Get configuration values from JSON file.
     """
     conf = {}
     with open(conf_file, 'r', encoding='utf-8') as stream:
         conf_string = io.StringIO(stream.read())
         conf_ini = configparser.ConfigParser()
         conf_ini.read_file(conf_string)
```

### Comparing `conflog-1.3.0/conflog.egg-info/PKG-INFO` & `conflog-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,25 +46,59 @@
       env: "dev"
       id: "123"
  
 And then use it in your Python code:
 
     from conflog import Conflog
 
-    cfl = conflog.Conflog(conf_files=['conflog.yaml'])
+    cfl = Conflog(conf_files=['conflog.yaml'])
     logger = cfl.get_logger('somename')
     logger.debug('Some debug message')
     logger.info('Some info message')
     logger.critical('Some critical message')
 
 It will write the log messages to stdout and file `conflog.log`:
 
     [SOMEAPP] [dev-123] 2023-06-07 10:49:01 INFO Some info message
     [SOMEAPP] [dev-123] 2023-06-07 10:49:52 CRITICAL Some critical message
 
+If you specify environment variables configuration, it will overwrite the configuration files:
+
+    import os
+    from conflog import Conflog
+
+    os.environ['CONFLOG_FORMAT'] = '[ENVAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s'
+    cfl = Conflog(conf_files=['conflog.yaml'])
+    logger.debug('Some debug message')
+    logger.info('Some info message')
+    logger.critical('Some critical message')
+
+It will write the log messages using the format from `CONFLOG_FORMAT` environment variable:
+
+    [ENVAPP] [dev-123] 2023-06-07 10:49:01 INFO Some info message
+    [ENVAPP] [dev-123] 2023-06-07 10:49:52 CRITICAL Some critical message
+
+And if you specify configuration dictionary, it will overwrite everything else:
+
+    import os
+    from conflog import Conflog
+
+    os.environ['CONFLOG_FORMAT'] = '[ENVAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s'
+    cfl = Conflog(
+        conf_files=['conflog.yaml'],
+        conf_dict={'format': '[DICTAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s'})
+    logger.debug('Some debug message')
+    logger.info('Some info message')
+    logger.critical('Some critical message')
+
+It will write the log messages using the format from configuration dictionary:
+
+    [DICTAPP] [dev-123] 2023-06-07 10:49:01 INFO Some info message
+    [DICTAPP] [dev-123] 2023-06-07 10:49:52 CRITICAL Some critical message
+
 Configuration
 -------------
 
 Configuration properties:
 
 | Property | Description | Default | Example |
 | -------- | ----------- | ------- | ------- |
@@ -72,15 +106,17 @@
 | datefmt | Date format | `%d-%b-%y %H:%M:%S` | `%Y-%m-%d %H:%M:%S` |
 | filename | Log file name | `conflog.log` | `someconflog.log` |
 | filemode | Log file mode | `w` | `w` |
 | format | Log message format | %(asctime)s --> %(name)s - %(levelname)s - %(message)s | `[SOMEAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s` |
 | level | Log level, supported values are `debug`, `info`, `warning`, `error`, `critical` | `info` | `critical` |
 | extras | Extra fields to be added to log message. It can be comma separated key value pairs with equal separator, or a key value pairs map for JSON and YAML configuration files | None | `env=dev,id=123` |
 
-Configuration files can be in YAML, JSON, XML, or INI format. Multiple files can be specified in the `conf_files` parameter when initialising `Conflog`, the configuration will be merged in the order of the files, the latter file will override the former file, and environment variables override configuration files' properties.
+Configuration files can be in YAML, JSON, XML, or INI format. Multiple files can be specified in the `conf_files` parameter when initialising `Conflog`, the configuration will be merged in the order of the files, the latter file will overwrites the former file.
+
+Environment variables configuration overwrites configuration files' properties. And finally, configuration dictionary overwrite everything else.
 
 ### YAML
 
 Example YAML configuration file:
 
     ---
     handlers: "stream,file"
@@ -149,15 +185,15 @@
     CONFLOG_FORMAT="[SOMEAPP] [%(env)s-%(id)s] %(asctime)s %(levelname)s %(message)s"
     CONFLOG_LEVEL="info"
     CONFLOG_EXTRAS="env=dev,id=123"
 
 Colophon
 --------
 
-[Developer's Guide](https://cliffano.github.io/developers_guide.html#nodejs)
+[Developer's Guide](https://cliffano.github.io/developers_guide.html#python)
 
 Build reports:
 
 * [Lint report](https://cliffano.github.io/pyconflog/lint/pylint/index.html)
 * [Code complexity report](https://cliffano.github.io/pyconflog/complexity/wily/index.html)
 * [Unit tests report](https://cliffano.github.io/pyconflog/test/pytest/index.html)
 * [Test coverage report](https://cliffano.github.io/pyconflog/coverage/coverage/index.html)
```

### Comparing `conflog-1.3.0/conflog.egg-info/SOURCES.txt` & `conflog-1.4.0/conflog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/setup.py` & `conflog-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/handlers/test_file_handler.py` & `conflog-1.4.0/tests/handlers/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/handlers/test_stream_handler.py` & `conflog-1.4.0/tests/handlers/test_stream_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/loaders/test_environ_loader.py` & `conflog-1.4.0/tests/loaders/test_environ_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/loaders/test_ini_loader.py` & `conflog-1.4.0/tests/loaders/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/loaders/test_json_loader.py` & `conflog-1.4.0/tests/loaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/loaders/test_xml_loader.py` & `conflog-1.4.0/tests/loaders/test_xml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/loaders/test_yaml_loader.py` & `conflog-1.4.0/tests/loaders/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.3.0/tests/test_config.py` & `conflog-1.4.0/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,57 +113,78 @@
                          'somelog %(asctime)s --> %(name)s - %(levelname)s - %(message)s')
         self.assertEqual(config.get_level(), logging.CRITICAL)
         extras = config.get_extras()
         self.assertEqual(len(extras.keys()), 2)
         self.assertEqual(extras['some_extra1'], 'some_value1')
         self.assertEqual(extras['some_extra2'], 'some_value2')
 
-    @patch('conflog.loaders.environ_loader.load')
+    @patch('conflog.loaders.yaml_loader.load')
     @patch('conflog.loaders.ini_loader.load')
-    def test_get_config_with_ini_overwritten_by_environ(self, func_ini, func_environ):
+    def test_get_config_with_ini_overwritten_by_yaml_sequence(self, func_ini, func_yaml):
         func_ini.return_value = CUSTOM_CONF
-        func_environ.return_value = OVERWRITE_CONF
-        config = Config(conf_files=['somefile.ini'])
+        func_yaml.return_value = OVERWRITE_CONF
+        config = Config(conf_files=['somefile.ini', 'somefile.yaml'])
         self.assertEqual(config.get_handlers(), ['stream', 'file'])
         self.assertEqual(config.get_datefmt(), '%d%m%y')
         self.assertEqual(config.get_filename(), 'overwriteconflog.log')
         self.assertEqual(config.get_filemode(), 'r')
         self.assertEqual(config.get_format(),
                          'overwritelog %(asctime)s --> %(name)s - %(levelname)s - %(message)s')
         self.assertEqual(config.get_level(), logging.DEBUG)
         extras = config.get_extras()
         self.assertEqual(len(extras.keys()), 1)
         self.assertEqual(extras['some_overwrite_extra1'], 'some_overwrite_value1')
 
-    @patch('conflog.loaders.yaml_loader.load')
     @patch('conflog.loaders.ini_loader.load')
-    def test_get_config_with_ini_overwritten_by_yaml(self, func_ini, func_yaml):
-        func_ini.return_value = CUSTOM_CONF
-        func_yaml.return_value = OVERWRITE_CONF
-        config = Config(conf_files=['somefile.ini', 'somefile.yaml'])
+    @patch('conflog.loaders.yaml_loader.load')
+    def test_get_config_with_yaml_overwritten_by_ini_sequence(self, func_yaml, func_ini):
+        func_yaml.return_value = CUSTOM_CONF
+        func_ini.return_value = OVERWRITE_CONF
+        config = Config(conf_files=['somefile.yaml', 'somefile.ini'])
         self.assertEqual(config.get_handlers(), ['stream', 'file'])
         self.assertEqual(config.get_datefmt(), '%d%m%y')
         self.assertEqual(config.get_filename(), 'overwriteconflog.log')
         self.assertEqual(config.get_filemode(), 'r')
         self.assertEqual(config.get_format(),
                          'overwritelog %(asctime)s --> %(name)s - %(levelname)s - %(message)s')
         self.assertEqual(config.get_level(), logging.DEBUG)
         extras = config.get_extras()
         self.assertEqual(len(extras.keys()), 1)
         self.assertEqual(extras['some_overwrite_extra1'], 'some_overwrite_value1')
 
+    @patch('conflog.loaders.environ_loader.load')
     @patch('conflog.loaders.ini_loader.load')
-    @patch('conflog.loaders.yaml_loader.load')
-    def test_get_config_with_yaml_overwritten_by_ini(self, func_yaml, func_ini):
-        func_yaml.return_value = CUSTOM_CONF
-        func_ini.return_value = OVERWRITE_CONF
-        config = Config(conf_files=['somefile.yaml', 'somefile.ini'])
+    def test_get_config_with_ini_overwritten_by_environ(self, func_ini, func_environ):
+        func_ini.return_value = CUSTOM_CONF
+        func_environ.return_value = OVERWRITE_CONF
+        config = Config(conf_files=['somefile.ini'])
         self.assertEqual(config.get_handlers(), ['stream', 'file'])
         self.assertEqual(config.get_datefmt(), '%d%m%y')
         self.assertEqual(config.get_filename(), 'overwriteconflog.log')
         self.assertEqual(config.get_filemode(), 'r')
         self.assertEqual(config.get_format(),
                          'overwritelog %(asctime)s --> %(name)s - %(levelname)s - %(message)s')
         self.assertEqual(config.get_level(), logging.DEBUG)
         extras = config.get_extras()
         self.assertEqual(len(extras.keys()), 1)
         self.assertEqual(extras['some_overwrite_extra1'], 'some_overwrite_value1')
+
+    @patch('conflog.loaders.environ_loader.load')
+    @patch('conflog.loaders.ini_loader.load')
+    def test_get_config_with_ini_overwritten_by_conf_dict(self, func_ini, func_environ):
+        func_ini.return_value = CUSTOM_CONF
+        func_environ.return_value = OVERWRITE_CONF
+        conf_dict = {
+            'handlers': 'stream',
+            'datefmt': '%y',
+            'filename': 'overwriteconfdictlog.log',
+            'filemode': 'w',
+            'format': '%(message)s',
+            'level': 'critical'
+        }
+        config = Config(conf_files=['somefile.ini'], conf_dict=conf_dict)
+        self.assertEqual(config.get_handlers(), ['stream'])
+        self.assertEqual(config.get_datefmt(), '%y')
+        self.assertEqual(config.get_filename(), 'overwriteconfdictlog.log')
+        self.assertEqual(config.get_filemode(), 'w')
+        self.assertEqual(config.get_format(), '%(message)s')
+        self.assertEqual(config.get_level(), logging.CRITICAL)
```

### Comparing `conflog-1.3.0/tests/test_conflog.py` & `conflog-1.4.0/tests/test_conflog.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,31 +39,40 @@
         func_get_logger.return_value = mock_logger
         func_logger_adapter.return_value = mock_adapted_logger
 
         mock_config.get_handlers.return_value = ['stream', 'file']
         mock_config.get_datefmt.return_value = '%d-%b-%y %H:%M:%S'
         mock_config.get_level.return_value = logging.INFO
 
-        conflog = Conflog(conf_files=['somefile.ini', 'somefile.json'])
+        conflog = Conflog(
+            conf_files=['somefile.ini', 'somefile.json'],
+            conf_dict={'format': '[SOMEAPP] %(message)s'}
+        )
         mock_stream_handler.setFormatter.assert_called_once_with(mock_formatter)
         mock_stream_handler.setLevel.assert_called_once_with(logging.INFO)
         mock_file_handler.setFormatter.assert_called_once_with(mock_formatter)
         mock_file_handler.setLevel.assert_called_once_with(logging.INFO)
         func_basic_config.assert_called_once_with(
             datefmt='%d-%b-%y %H:%M:%S',
             level=logging.INFO,
         )
 
         logger = conflog.get_logger('someloggername')
         func_get_logger.assert_called_with('someloggername')
         self.assertEqual(logger, mock_adapted_logger)
         self.assertFalse(mock_logger.propagate)
+
+        # should add configured handlers
         mock_logger.addHandler.assert_any_call(mock_stream_handler)
         mock_logger.addHandler.assert_any_call(mock_file_handler)
+
+        # should set configured log level
         mock_adapted_logger.setLevel.assert_called_once_with(logging.INFO)
 
         conflog.close_logger_handlers('someloggername')
+        # should close configured handlers
         mock_stream_handler.close.assert_called_once_with()
         mock_file_handler.close.assert_called_once_with()
 
         config = conflog.get_config_properties()
+        # should retrieve the correct configuration
         self.assertEqual(config, mock_config.conf)
```

