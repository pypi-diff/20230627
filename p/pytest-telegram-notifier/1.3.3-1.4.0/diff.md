# Comparing `tmp/pytest-telegram-notifier-1.3.3.tar.gz` & `tmp/pytest-telegram-notifier-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-telegram-notifier-1.3.3.tar", last modified: Fri Mar 17 17:38:46 2023, max compression
+gzip compressed data, was "pytest-telegram-notifier-1.4.0.tar", last modified: Tue Jun 27 09:26:24 2023, max compression
```

## Comparing `pytest-telegram-notifier-1.3.3.tar` & `pytest-telegram-notifier-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:46.614203 pytest-telegram-notifier-1.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:46.610203 pytest-telegram-notifier-1.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:46.610203 pytest-telegram-notifier-1.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-03-17 17:38:46.614203 pytest-telegram-notifier-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:46.610203 pytest-telegram-notifier-1.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    70055 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/docs/telegram-message.png
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/pytest-telegram-notifier.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:46.610203 pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-03-17 17:38:46.000000 pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-17 17:38:46.000000 pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 17:38:46.000000 pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-17 17:38:46.000000 pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-17 17:38:46.000000 pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 17:38:46.614203 pytest-telegram-notifier-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:46.614203 pytest-telegram-notifier-1.3.3/telegram_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-17 17:38:46.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-17 17:38:27.000000 pytest-telegram-notifier-1.3.3/telegram_notifier/telegram_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:24.798341 pytest-telegram-notifier-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:24.794341 pytest-telegram-notifier-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:24.794341 pytest-telegram-notifier-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-27 09:26:24.794341 pytest-telegram-notifier-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:24.794341 pytest-telegram-notifier-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    70055 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/docs/telegram-message.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/pytest-telegram-notifier.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:24.794341 pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-27 09:26:24.000000 pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 09:26:24.000000 pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:26:24.000000 pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 09:26:24.000000 pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 09:26:24.000000 pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:26:24.798341 pytest-telegram-notifier-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:24.794341 pytest-telegram-notifier-1.4.0/telegram_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 09:26:24.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-27 09:26:13.000000 pytest-telegram-notifier-1.4.0/telegram_notifier/telegram_manager.py
```

### Comparing `pytest-telegram-notifier-1.3.3/.github/workflows/main.yml` & `pytest-telegram-notifier-1.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/.gitignore` & `pytest-telegram-notifier-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/.pre-commit-config.yaml` & `pytest-telegram-notifier-1.4.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
   python: python3
 repos:
   - repo: https://github.com/dannysepler/rm_unneeded_f_str
     rev: v0.2.0
     hooks:
     -   id: rm-unneeded-f-str
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     - id: black
       language_version: python3.9
   - repo: https://github.com/hadialqattan/pycln
-    rev: v2.1.3
+    rev: v2.1.5
     hooks:
       - id: pycln
         args: [ --config=pyproject.toml ]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-ast
```

### Comparing `pytest-telegram-notifier-1.3.3/LICENSE.rst` & `pytest-telegram-notifier-1.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/PKG-INFO` & `pytest-telegram-notifier-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-telegram-notifier
-Version: 1.3.3
+Version: 1.4.0
 Summary: Telegram notification plugin for Pytest
 Author-email: Kirill Matveev <matveevkirill@internet.ru>
 Maintainer-email: Kirill Matveev <matveevkirill@internet.ru>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pytest-telegram-notifier-1.3.3/README.md` & `pytest-telegram-notifier-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/docs/telegram-message.png` & `pytest-telegram-notifier-1.4.0/docs/telegram-message.png`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/pyproject.toml` & `pytest-telegram-notifier-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/PKG-INFO` & `pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-telegram-notifier
-Version: 1.3.3
+Version: 1.4.0
 Summary: Telegram notification plugin for Pytest
 Author-email: Kirill Matveev <matveevkirill@internet.ru>
 Maintainer-email: Kirill Matveev <matveevkirill@internet.ru>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pytest-telegram-notifier-1.3.3/pytest_telegram_notifier.egg-info/SOURCES.txt` & `pytest-telegram-notifier-1.4.0/pytest_telegram_notifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/telegram_notifier/bot.py` & `pytest-telegram-notifier-1.4.0/telegram_notifier/bot.py`

 * *Files identical despite different names*

### Comparing `pytest-telegram-notifier-1.3.3/telegram_notifier/plugin.py` & `pytest-telegram-notifier-1.4.0/telegram_notifier/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from _pytest.config.argparsing import Parser
-from _pytest.fixtures import Config, FixtureRequest
+from _pytest.fixtures import Config
 from pluggy import PluginManager
 
 from . import hooks
-from .telegram_manager import TelegramManager, TelegramManagerAdditionalFieldsWorker
+from .telegram_manager import TelegramManager
 
 
 def pytest_addoption(parser: Parser):
     group = parser.getgroup('telegram_notifier')
     group.addoption(
         '--telegram-notifier',
         action='store_true',
@@ -22,24 +22,12 @@
     )
 
 
 def pytest_addhooks(pluginmanager: PluginManager):
     pluginmanager.add_hookspecs(hooks)
 
 
-def pytest_configure(config: Config):
-    if not config.option.telegram_notifier:
-        return
-
-    if not hasattr(config, 'workerinput'):
+@pytest.mark.tryfirst
+def pytest_cmdline_main(config: Config):
+    if config.option.telegram_notifier:
         manager = TelegramManager(config)
         config.pluginmanager.register(manager, 'pytest_telegram_notifier')
-
-
-def pytest_unconfigure(config: Config):
-    if not hasattr(config, 'workerinput'):
-        config.pluginmanager.unregister(name='pytest_telegram_notifier')
-
-
-@pytest.fixture(scope='session')
-def telegram_notifier_bot(request: FixtureRequest) -> TelegramManagerAdditionalFieldsWorker:
-    return request.config.pluginmanager.get_plugin('pytest_telegram_notifier').additional_fields_worker
```

### Comparing `pytest-telegram-notifier-1.3.3/telegram_notifier/telegram_manager.py` & `pytest-telegram-notifier-1.4.0/telegram_notifier/telegram_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=W0212
 
 import copy
 from datetime import datetime
 
 import pytest
-from _pytest.config import Config
+from _pytest.config import Config, ExitCode
 from _pytest.main import Session
 from _pytest.reports import TestReport
 
 from telegram_notifier.bot import CallModeEnum, TelegramBot
 from telegram_notifier.exceptions import TelegramNotifierError
 
 
@@ -30,14 +30,15 @@
 
 class TelegramManager:
     def __init__(self, config: Config):
         self.datetime_start_tests = None
         self.testsskipped = 0
         self.testsfailed = 0
         self.testscollected = 0
+        self.exitstatus = None
 
         self._config = config
         self._additional_fields_worker = TelegramManagerAdditionalFieldsWorker()
 
     @property
     def additional_fields_worker(self) -> TelegramManagerAdditionalFieldsWorker:
         return self._additional_fields_worker
@@ -81,19 +82,26 @@
 
     @pytest.hookimpl(trylast=True)
     def pytest_sessionstart(self):
         self.datetime_start_tests = datetime.now()
 
     @pytest.hookimpl(trylast=True)
     def pytest_sessionfinish(self, session: Session):
+        self.exitstatus = session.exitstatus
         self.testsfailed = session.testsfailed
         self.testscollected = session.testscollected
 
     @pytest.hookimpl(trylast=True)
     def pytest_unconfigure(self):
+        if hasattr(self._config, 'workerinput'):
+            return
+
+        if self.exitstatus in [ExitCode.INTERNAL_ERROR, ExitCode.USAGE_ERROR, ExitCode.INTERRUPTED]:
+            self.testsfailed = self.testscollected
+
         telegram_bot = TelegramBot(self._config.option.telegram_notifier_config_file)
 
         self._config.hook.pytest_telegram_notifier_message_additional_fields(config=self._config)
         self._additional_fields_worker.register_additional_fields(
             dict(self._config.stash.get('telegram-notifier-addfields', {})),
         )
```

