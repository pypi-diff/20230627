# Comparing `tmp/xirvik_tools-0.4.0.tar.gz` & `tmp/xirvik_tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xirvik_tools-0.4.0.tar", max compression
+gzip compressed data, was "xirvik_tools-0.4.1.tar", max compression
```

## Comparing `xirvik_tools-0.4.0.tar` & `xirvik_tools-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2015-04-05 10:25:34.116301 xirvik_tools-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      628 2023-04-11 15:59:06.810994 xirvik_tools-0.4.0/LaunchAgents/README.md
--rw-r--r--   0        0        0      733 2023-04-14 20:37:57.649077 xirvik_tools-0.4.0/LaunchAgents/sh.tat.XirvikStartTorrents.plist
--rw-r--r--   0        0        0      297 2021-09-30 10:40:35.069636 xirvik_tools-0.4.0/README.md
--rw-r--r--   0        0        0     1509 2023-06-26 20:04:24.702376 xirvik_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      815 2020-02-20 00:53:15.113538 xirvik_tools-0.4.0/systemd/README.md
--rw-r--r--   0        0        0      140 2021-09-12 02:01:33.922925 xirvik_tools-0.4.0/systemd/xirvik-start-torrents.service
--rw-r--r--   0        0        0      128 2020-02-20 00:53:15.113538 xirvik_tools-0.4.0/systemd/xirvik-start-torrents.timer
--rw-r--r--   0        0        0       95 2020-10-29 09:51:37.765849 xirvik_tools-0.4.0/xirvik/__init__.py
--rw-r--r--   0        0        0    15074 2023-06-26 20:04:24.702376 xirvik_tools-0.4.0/xirvik/client.py
--rw-r--r--   0        0        0       71 2021-09-14 05:10:34.682258 xirvik_tools-0.4.0/xirvik/commands/__init__.py
--rw-r--r--   0        0        0     4104 2023-04-14 20:32:03.847391 xirvik_tools-0.4.0/xirvik/commands/delete_old.py
--rw-r--r--   0        0        0     3841 2023-05-25 22:51:02.179751 xirvik_tools-0.4.0/xirvik/commands/move_by_label.py
--rw-r--r--   0        0        0     2936 2023-04-14 20:32:03.841391 xirvik_tools-0.4.0/xirvik/commands/move_erroneous.py
--rw-r--r--   0        0        0     1710 2023-04-14 20:32:03.847391 xirvik_tools-0.4.0/xirvik/commands/root.py
--rw-r--r--   0        0        0    18568 2023-04-14 20:37:57.649077 xirvik_tools-0.4.0/xirvik/commands/simple.py
--rw-r--r--   0        0        0     7017 2023-04-16 21:50:00.051679 xirvik_tools-0.4.0/xirvik/commands/util.py
--rw-r--r--   0        0        0     2412 2023-04-14 20:37:57.649077 xirvik_tools-0.4.0/xirvik/typing.py
--rw-r--r--   0        0        0     1065 2023-06-26 20:04:24.702376 xirvik_tools-0.4.0/xirvik/utils.py
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 xirvik_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2015-04-05 10:25:34.116301 xirvik_tools-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0      628 2023-04-11 15:59:06.810994 xirvik_tools-0.4.1/LaunchAgents/README.md
+-rw-r--r--   0        0        0      733 2023-04-14 20:37:57.649077 xirvik_tools-0.4.1/LaunchAgents/sh.tat.XirvikStartTorrents.plist
+-rw-r--r--   0        0        0      297 2021-09-30 10:40:35.069636 xirvik_tools-0.4.1/README.md
+-rw-r--r--   0        0        0     1510 2023-06-27 10:47:01.640583 xirvik_tools-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      815 2020-02-20 00:53:15.113538 xirvik_tools-0.4.1/systemd/README.md
+-rw-r--r--   0        0        0      140 2021-09-12 02:01:33.922925 xirvik_tools-0.4.1/systemd/xirvik-start-torrents.service
+-rw-r--r--   0        0        0      128 2020-02-20 00:53:15.113538 xirvik_tools-0.4.1/systemd/xirvik-start-torrents.timer
+-rw-r--r--   0        0        0       95 2020-10-29 09:51:37.765849 xirvik_tools-0.4.1/xirvik/__init__.py
+-rw-r--r--   0        0        0    15074 2023-06-26 20:04:24.702376 xirvik_tools-0.4.1/xirvik/client.py
+-rw-r--r--   0        0        0       71 2021-09-14 05:10:34.682258 xirvik_tools-0.4.1/xirvik/commands/__init__.py
+-rw-r--r--   0        0        0     4104 2023-04-14 20:32:03.847391 xirvik_tools-0.4.1/xirvik/commands/delete_old.py
+-rw-r--r--   0        0        0     3841 2023-05-25 22:51:02.179751 xirvik_tools-0.4.1/xirvik/commands/move_by_label.py
+-rw-r--r--   0        0        0     2936 2023-04-14 20:32:03.841391 xirvik_tools-0.4.1/xirvik/commands/move_erroneous.py
+-rw-r--r--   0        0        0     1710 2023-04-14 20:32:03.847391 xirvik_tools-0.4.1/xirvik/commands/root.py
+-rw-r--r--   0        0        0    18568 2023-04-14 20:37:57.649077 xirvik_tools-0.4.1/xirvik/commands/simple.py
+-rw-r--r--   0        0        0     7057 2023-06-27 10:46:50.150599 xirvik_tools-0.4.1/xirvik/commands/util.py
+-rw-r--r--   0        0        0     2412 2023-04-14 20:37:57.649077 xirvik_tools-0.4.1/xirvik/typing.py
+-rw-r--r--   0        0        0     1065 2023-06-26 20:04:24.702376 xirvik_tools-0.4.1/xirvik/utils.py
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 xirvik_tools-0.4.1/PKG-INFO
```

### Comparing `xirvik_tools-0.4.0/LICENSE.txt` & `xirvik_tools-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/LaunchAgents/README.md` & `xirvik_tools-0.4.1/LaunchAgents/README.md`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/LaunchAgents/sh.tat.XirvikStartTorrents.plist` & `xirvik_tools-0.4.1/LaunchAgents/sh.tat.XirvikStartTorrents.plist`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/pyproject.toml` & `xirvik_tools-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 homepage = "https://github.com/Tatsh/xirvik-tools"
 include = ["LaunchAgents", "systemd"]
 keywords = ["command line", "utilities", "xirvik"]
 license = "MIT"
 name = "xirvik-tools"
 packages = [{ include = "xirvik" }]
 readme = "README.md"
-version = "0.4.0"
+version = "0.4.1"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 unidecode = "^1.3.6"
 beautifulsoup4 = "^4.12.1"
 cached-property = "^1.5.2"
 click = "^8.1.3"
 html5lib = "^1.1"
 loguru = "^0.7.0"
 pyyaml = "^6.0"
 requests = "^2.31.0"
 tabulate = "^0.9.0"
 urllib3 = "^2.0.3"
-xdg = "^6.0.0"
+pyxdg = "^0.28"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `xirvik_tools-0.4.0/systemd/README.md` & `xirvik_tools-0.4.1/systemd/README.md`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/client.py` & `xirvik_tools-0.4.1/xirvik/client.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/commands/delete_old.py` & `xirvik_tools-0.4.1/xirvik/commands/delete_old.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/commands/move_by_label.py` & `xirvik_tools-0.4.1/xirvik/commands/move_by_label.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/commands/move_erroneous.py` & `xirvik_tools-0.4.1/xirvik/commands/move_erroneous.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/commands/root.py` & `xirvik_tools-0.4.1/xirvik/commands/root.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/commands/simple.py` & `xirvik_tools-0.4.1/xirvik/commands/simple.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/commands/util.py` & `xirvik_tools-0.4.1/xirvik/commands/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 import sys
 import warnings
 
 from click.core import ParameterSource
 from loguru import logger
 import click
-import xdg
+import xdg.BaseDirectory
 import yaml
 
 __all__ = ('common_options_and_arguments', 'complete_hosts', 'complete_ports',
            'setup_log_intercept_handler', 'setup_logging')
 
 
 def setup_logging(debug: bool | None = False) -> None:
@@ -142,15 +142,15 @@
     config_file_param_name : str
         The name of the parameter given to Click in ``click.option``.
 
     default_section : str | None
         Default top key of YAML to read from.
     """
     home = pathlib.Path.home()
-    default_config_file_path = xdg.xdg_config_home() / 'xirvik.yml'
+    default_config_file_path = pathlib.Path(xdg.BaseDirectory.xdg_config_home) / 'xirvik.yml'
     if sys.platform == 'win32':  # pragma: no cover
         default_config_file_path = home / 'AppData/Roaming/xirvik-tools/config.yml'
     elif sys.platform == 'darwin':  # pragma: no cover
         default_config_file_path = home / 'Library/Application Support/xirvik-tools/config.yml'
 
     class _ConfigFileCommand(click.Command):
         def invoke(self, ctx: click.Context) -> Any:
```

### Comparing `xirvik_tools-0.4.0/xirvik/typing.py` & `xirvik_tools-0.4.1/xirvik/typing.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/xirvik/utils.py` & `xirvik_tools-0.4.1/xirvik/utils.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.0/PKG-INFO` & `xirvik_tools-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xirvik-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command line utilities for interfacing with Xirvik.
 Home-page: https://github.com/Tatsh/xirvik-tools
 License: MIT
 Keywords: command line,utilities,xirvik
 Author: Fa An
 Author-email: 2998784916@qq.com
 Requires-Python: >=3.10,<4.0
@@ -14,20 +14,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pyxdg (>=0.28,<0.29)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: unidecode (>=1.3.6,<2.0.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
-Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Project-URL: Documentation, https://xirvik-tools.readthedocs.io/
 Description-Content-Type: text/markdown
 
 # Something here
 
 ![Lint](https://github.com/Tatsh/xirvik-tools/workflows/Lint/badge.svg)
 ![Tests](https://github.com/Tatsh/xirvik-tools/workflows/Tests/badge.svg)
```

