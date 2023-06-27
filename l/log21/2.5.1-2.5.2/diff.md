# Comparing `tmp/log21-2.5.1.tar.gz` & `tmp/log21-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.5.1.tar", last modified: Thu Jun  8 18:34:10 2023, max compression
+gzip compressed data, was "log21-2.5.2.tar", last modified: Tue Jun 27 02:58:12 2023, max compression
```

## Comparing `log21-2.5.1.tar` & `log21-2.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:10.165571 log21-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-08 18:33:59.000000 log21-2.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-06-08 18:34:10.165571 log21-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-08 18:33:59.000000 log21-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:10.165571 log21-2.5.1/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-06-08 18:33:59.000000 log21-2.5.1/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-08 18:33:59.000000 log21-2.5.1/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:10.165571 log21-2.5.1/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-08 18:33:59.000000 log21-2.5.1/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-08 18:33:59.000000 log21-2.5.1/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 18:33:59.000000 log21-2.5.1/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 18:33:59.000000 log21-2.5.1/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-06-08 18:33:59.000000 log21-2.5.1/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-08 18:33:59.000000 log21-2.5.1/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-08 18:33:59.000000 log21-2.5.1/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-06-08 18:33:59.000000 log21-2.5.1/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-08 18:33:59.000000 log21-2.5.1/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-06-08 18:33:59.000000 log21-2.5.1/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-06-08 18:33:59.000000 log21-2.5.1/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-08 18:33:59.000000 log21-2.5.1/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-08 18:33:59.000000 log21-2.5.1/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21423 2023-06-08 18:33:59.000000 log21-2.5.1/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:10.165571 log21-2.5.1/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-06-08 18:34:10.000000 log21-2.5.1/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-08 18:34:10.000000 log21-2.5.1/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:34:10.000000 log21-2.5.1/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:34:10.000000 log21-2.5.1/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 18:34:10.000000 log21-2.5.1/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-08 18:33:59.000000 log21-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:34:10.165571 log21-2.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-27 02:58:02.000000 log21-2.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-27 02:58:12.259999 log21-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-27 02:58:02.000000 log21-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21666 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 02:58:02.000000 log21-2.5.2/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-27 02:58:02.000000 log21-2.5.2/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-27 02:58:02.000000 log21-2.5.2/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 02:58:02.000000 log21-2.5.2/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-06-27 02:58:02.000000 log21-2.5.2/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-06-27 02:58:02.000000 log21-2.5.2/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-27 02:58:02.000000 log21-2.5.2/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-27 02:58:02.000000 log21-2.5.2/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-27 02:58:02.000000 log21-2.5.2/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-27 02:58:02.000000 log21-2.5.2/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-27 02:58:02.000000 log21-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 02:58:12.259999 log21-2.5.2/setup.cfg
```

### Comparing `log21-2.5.1/LICENSE.txt` & `log21-2.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/PKG-INFO` & `log21-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.1
+Version: 2.5.2
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
@@ -71,17 +71,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.1
+### 2.5.2
 
-Switched from `setup.py` build system to `pyproject.toml`
+Improved type-hintings.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.1/README.md` & `log21-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.1
+### 2.5.2
 
-Switched from `setup.py` build system to `pyproject.toml`
+Improved type-hintings.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.1/log21/Argparse.py` & `log21-2.5.2/log21/Argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # log21.Argparse.py
 # CodeWriter21
 
 import re as _re
 import sys as _sys
 import log21 as _log21
 import argparse as _argparse
-from typing import Mapping as _Mapping
+
 from gettext import gettext as _gettext
 from textwrap import TextWrapper as _TextWrapper
+from typing import Mapping as _Mapping, Optional as _Optional
+
 from log21.Colors import get_colors as _gc
 from log21.Formatters import DecolorizingFormatter as _Formatter
 
 __all__ = ['ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper']
 
 
 class ColorizingHelpFormatter(_argparse.HelpFormatter):
@@ -473,15 +475,15 @@
                         lines.append(indent + self.placeholder.lstrip())
                     break
 
         return lines
 
 
 class ColorizingArgumentParser(_argparse.ArgumentParser):
-    def __init__(self, formatter_class=ColorizingHelpFormatter, colors: _Mapping[str, str] = None, **kwargs):
+    def __init__(self, formatter_class=ColorizingHelpFormatter, colors: _Optional[_Mapping[str, str]] = None, **kwargs):
         self.logger = _log21.Logger('ArgumentParser')
         self.colors = colors
         super().__init__(formatter_class=formatter_class, **kwargs)
 
     def _print_message(self, message, file=None):
         if message:
             self.logger.handlers.clear()
```

### Comparing `log21-2.5.1/log21/Colors.py` & `log21-2.5.2/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/log21/CrashReporter/Formatters.py` & `log21-2.5.2/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/log21/CrashReporter/Reporters.py` & `log21-2.5.2/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/log21/FileHandler.py` & `log21-2.5.2/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/log21/Formatters.py` & `log21-2.5.2/log21/Formatters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # log21.Formatters.py
 # CodeWriter21
 
 import time as _time
 from logging import Formatter as __Formatter
-from typing import Mapping as _Mapping, Tuple as _Tuple
+from typing import Mapping as _Mapping, Tuple as _Tuple, Dict as _Dict, Optional as _Optional
 from log21.Colors import get_colors as _gc, ansi_escape
 from log21.Levels import INPUT, CRITICAL, ERROR, WARNING, INFO, DEBUG, PRINT
 
 __all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
 
 
 class _Formatter(__Formatter):
-    _level_names: _Mapping[int, str] = {
+    _level_names: _Dict[int, str] = {
         DEBUG: 'DEBUG',
         INFO: 'INFO',
         WARNING: 'WARNING',
         ERROR: 'ERROR',
         CRITICAL: 'CRITICAL',
         PRINT: 'PRINT',
         INPUT: 'INPUT'
     }
 
-    def __init__(self, fmt: str = None, datefmt: str = None, style: str = '%', level_names: _Mapping[int, str] = None):
+    def __init__(self, fmt: _Optional[str] = None, datefmt: _Optional[str] = None, style: str = '%',
+                 level_names: _Optional[_Mapping[int, str]] = None):
         """
         `level_names` usage:
         >>> import log21
         >>> logger = log21.Logger('MyLogger', log21.DEBUG)
         >>> stream_handler = log21.ColorizingStreamHandler()
         >>> formatter = log21.ColorizingFormatter(fmt='[%(levelname)s] %(message)s',
         ...             level_names={log21.DEBUG: ' ', log21.INFO: '+', log21.WARNING: '-', log21.ERROR: '!',
@@ -53,15 +54,15 @@
                 self.level_names[level] = name
 
     @property
     def level_names(self):
         return self._level_names
 
     @level_names.setter
-    def level_names(self, level_names):
+    def level_names(self, level_names: _Mapping[int, str]):
         if level_names:
             if not isinstance(level_names, _Mapping):
                 raise TypeError('`level_names` must be a Mapping, a dictionary like object!')
             self._level_names = level_names
         else:
             self._level_names = dict()
 
@@ -85,33 +86,35 @@
                 s = s + "\n"
             s = s + self.formatStack(record.stack_info)
         return s
 
 
 class ColorizingFormatter(_Formatter):
     # Default color values
-    level_colors: _Mapping[int, _Tuple[str, ...]] = {
+    level_colors: _Dict[int, _Tuple[str, ...]] = {
         DEBUG: ('lightblue',),
         INFO: ('green',),
         WARNING: ('lightyellow',),
         ERROR: ('light red',),
         CRITICAL: ('background red', 'white'),
         PRINT: ('Cyan',),
         INPUT: ('Magenta',)
     }
     time_color: _Tuple[str, ...] = ('lightblue',)
     name_color = pathname_color = filename_color = module_color = func_name_color = thread_name_color = \
         message_color = tuple()
 
-    def __init__(self, fmt: str = None, datefmt: str = None, style: str = '%', level_names: _Mapping[int, str] = None,
-                 level_colors: _Mapping[int, _Tuple[str]] = None,
-                 time_color: _Tuple[str, ...] = None, name_color: _Tuple[str, ...] = None,
-                 pathname_color: _Tuple[str, ...] = None, filename_color: _Tuple[str, ...] = None,
-                 module_color: _Tuple[str, ...] = None, func_name_color: _Tuple[str, ...] = None,
-                 thread_name_color: _Tuple[str, ...] = None, message_color: _Tuple[str, ...] = None):
+    def __init__(self, fmt: _Optional[str] = None, datefmt: _Optional[str] = None, style: str = '%',
+                 level_names: _Optional[_Mapping[int, str]] = None,
+                 level_colors: _Optional[_Mapping[int, _Tuple[str]]] = None,
+                 time_color: _Optional[_Tuple[str, ...]] = None, name_color: _Optional[_Tuple[str, ...]] = None,
+                 pathname_color: _Optional[_Tuple[str, ...]] = None, filename_color: _Optional[_Tuple[str, ...]] = None,
+                 module_color: _Optional[_Tuple[str, ...]] = None, func_name_color: _Optional[_Tuple[str, ...]] = None,
+                 thread_name_color: _Optional[_Tuple[str, ...]] = None,
+                 message_color: _Optional[_Tuple[str, ...]] = None):
         super().__init__(fmt=fmt, datefmt=datefmt, style=style, level_names=level_names)
         # Checks and sets colors
         if level_colors:
             if not isinstance(level_colors, _Mapping):
                 raise TypeError('`level_colors` must be a dictionary like object!')
             for level, color in level_colors.items():
                 self.level_colors[level] = (_gc(*color),)
```

### Comparing `log21-2.5.1/log21/Logger.py` & `log21-2.5.2/log21/Logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # log21.Logger.py
 # CodeWriter21
 
 import logging as _logging
 
 from getpass import getpass as _getpass
-from typing import Sequence as _Sequence, Union as _Union
+from typing import Sequence as _Sequence, Union as _Union, Optional as _Optional, Callable as _Callable
 from logging import raiseExceptions as _raiseExceptions
 
 import log21 as _log21
 from log21.Levels import CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET, PRINT, INPUT
 
 __all__ = ['Logger']
 
 
 class Logger(_logging.Logger):
-    def __init__(self, name, level=NOTSET, handlers: _Union[_Sequence[_logging.Handler], _logging.Handler] = None):
+    def __init__(self, name, level: _Union[int, str]=NOTSET,
+                 handlers: _Optional[_Union[_Sequence[_logging.Handler], _logging.Handler]] = None):
         super().__init__(name, level)
         self.setLevel(level)
         self._progress_bar = None
         if handlers:
             if not isinstance(handlers, _Sequence):
                 if isinstance(handlers, _logging.Handler):
                     handlers = [handlers]
@@ -188,17 +189,17 @@
             self._progress_bar = ProgressBar(logger=self)
         return self._progress_bar
 
     @progress_bar.setter
     def progress_bar(self, value: '_log21.ProgressBar'):
         self._progress_bar = value
 
-    def clear_line(self, length: int = None):
+    def clear_line(self, length: _Optional[int] = None):
         """
         Clear the current line.
 
         :param length: The length of the line to clear.
         :return:
         """
         for handler in self.handlers:
-            if hasattr(handler, 'clear_line'):
+            if isinstance(getattr(handler, 'clear_line', None), _Callable):
                 handler.clear_line(length)
```

### Comparing `log21-2.5.1/log21/LoggingWindow.py` & `log21-2.5.2/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/log21/Manager.py` & `log21-2.5.2/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/log21/PPrint.py` & `log21-2.5.2/log21/PPrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import re as _re
 import sys as _sys
 import types as _types
 import collections as _collections
 import dataclasses as _dataclasses
 
-from typing import Mapping as _Mapping, Union as _Union
 from pprint import PrettyPrinter as _PrettyPrinter
+from typing import Mapping as _Mapping, Optional as _Optional
 
 from log21.Colors import get_colors as _gc
 
 _builtin_scalars = frozenset({str, bytes, bytearray, float, complex, bool, type(None)})
 
 
 def _recursion(obj):
@@ -71,16 +71,16 @@
         'parenthesis': _gc('LightGreen'),
         'comma': _gc('LightRed'),
         'colon': _gc('LightRed'),
         '...': _gc('LightMagenta'),
         'data': _gc('Green')
     }
 
-    def __init__(self, indent=1, width=80, depth=None, stream=None, signs_colors: _Mapping[str, str] = None, *,
-                 compact=False, sort_dicts=True, underscore_numbers=False, **kwargs):
+    def __init__(self, indent=1, width=80, depth=None, stream=None, signs_colors: _Optional[_Mapping[str, str]] = None,
+                 *, compact=False, sort_dicts=True, underscore_numbers=False, **kwargs):
         super().__init__(indent=indent, width=width, depth=depth, stream=stream, compact=compact, **kwargs)
         self._depth = depth
         self._indent_per_level = indent
         self._width = width
         if stream is not None:
             self._stream = stream
         else:
@@ -558,12 +558,12 @@
 
     def _pprint_user_string(self, obj, stream, indent, allowance, context, level):
         self._format(obj.data, stream, indent, allowance, context, level - 1)
 
     _dispatch[_collections.UserString.__repr__] = _pprint_user_string
 
 
-def pformat(obj, indent=1, width=80, depth=None, signs_colors: _Mapping[str, str] = None, *, compact=False,
+def pformat(obj, indent=1, width=80, depth=None, signs_colors: _Optional[_Mapping[str, str]] = None, *, compact=False,
             sort_dicts=True, underscore_numbers=False, **kwargs):
     """Format a Python object into a pretty-printed representation."""
     return PrettyPrinter(indent=indent, width=width, depth=depth, compact=compact, signs_colors=signs_colors,
-                         sort_dicts=True, underscore_numbers=False, **kwargs).pformat(obj)
+                         sort_dicts=sort_dicts, underscore_numbers=underscore_numbers, **kwargs).pformat(obj)
```

### Comparing `log21-2.5.1/log21/ProgressBar.py` & `log21-2.5.2/log21/ProgressBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # log21.ProgressBar.py
 # CodeWriter21
 
+from __future__ import annotations
+
 import shutil as _shutil
 
-from typing import Mapping as _Mapping, Any as _Any
+from typing import Mapping as _Mapping, Any as _Any, Optional as _Optional
 
 import log21 as _log21
 from log21.Logger import Logger as _Logger
 from log21.StreamHandler import ColorizingStreamHandler as _ColorizingStreamHandler
 from log21.Colors import get_colors as _gc
 
 _logger = _Logger('ProgressBar')
@@ -35,18 +37,18 @@
         ...     time.sleep(0.01)
         ...
         |████████████████████████████████████████████████████████████████████████████████████████████| 100%
         >>> # Of course, You should try it yourself to see the progress! XD
         >>>
     """
 
-    def __init__(self, *args, width: int = None, show_percentage: bool = True, prefix: str = '|', suffix: str = '|',
-                 fill: str = '█', empty: str = ' ', format_: str = None, style: str = '%',
-                 new_line_when_complete: bool = True, colors: dict = None, no_color: bool = False,
-                 logger: '_log21.Logger' = _logger, additional_variables: _Mapping[str, _Any] = None):
+    def __init__(self, *, width: _Optional[int] = None, show_percentage: bool = True, prefix: str = '|',
+                 suffix: str = '|', fill: str = '█', empty: str = ' ', format_: _Optional[str] = None, style: str = '%',
+                 new_line_when_complete: bool = True, colors: _Optional[_Mapping[str, str]] = None, no_color: bool = False,
+                 logger: _log21.Logger = _logger, additional_variables: _Optional[_Mapping[str, _Any]] = None):
         """
         :param args: Prevents the use of positional arguments
         :param width: The width of the progress bar
         :param show_percentage: Whether to show the percentage of the progress
         :param prefix: The prefix of the progress bar
         :param suffix: The suffix of the progress bar
         :param fill: The fill character of the progress bar
@@ -270,15 +272,15 @@
         elif self.style == '{':
             bar = self.format.format(**progress_dict)
         else:
             raise ValueError('`style` must be either `%` or `{`')
 
         return '\r' + bar + self.colors['reset-color'] + ('\n' if self.new_line_when_complete else '')
 
-    def __call__(self, progress: float, total: float, logger: '_log21.Logger' = None, **kwargs):
+    def __call__(self, progress: float, total: float, logger: _Optional[_log21.Logger] = None, **kwargs):
         if not logger:
             logger = self.logger
 
         logger.print(self.get_bar(progress, total, **kwargs), end='')
 
-    def update(self, progress: float, total: float, logger: '_log21.Logger' = None, **kwargs):
+    def update(self, progress: float, total: float, logger: _Optional[_log21.Logger] = None, **kwargs):
         self(progress, total, logger, **kwargs)
```

### Comparing `log21-2.5.1/log21/StreamHandler.py` & `log21-2.5.2/log21/StreamHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # CodeWriter21
 
 import os as _os
 import re as _re
 import shutil as _shutil
 
 from logging import StreamHandler as _StreamHandler
+from typing import Optional as _Optional
 from log21.Colors import ansi_escape as _ansi_escape, get_colors as _gc, hex_escape as _hex_escape
 
 __all__ = ['IS_WINDOWS', 'ColorizingStreamHandler', 'StreamHandler']
 
 IS_WINDOWS = _os.name == 'nt'
 
 if IS_WINDOWS:
@@ -55,15 +56,15 @@
     def emit(self, record):
         if self.HandleCR:
             self.check_cr(record)
         if self.HandleNL:
             self.check_nl(record)
         super().emit(record)
 
-    def clear_line(self, length: int = None):
+    def clear_line(self, length: _Optional[int] = None):
         """
         Clear the current line.
 
         :param length: The length of the line to clear.
         :return:
         """
         file_descriptor = getattr(self.stream, 'fileno', None)
```

### Comparing `log21-2.5.1/log21/TreePrint.py` & `log21-2.5.2/log21/TreePrint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # log21.TreePrint.py
 # CodeWriter21
 
-from typing import Union as _Union, Mapping as _Mapping, Sequence as _Sequence
+from __future__ import annotations
+
+from typing import Union as _Union, Mapping as _Mapping, Sequence as _Sequence, Optional as _Optional, List as _List
 
 from log21.Colors import get_colors as _gc
 
 
 class TreePrint:
     class Node:
         colors = {
             'branches': _gc('Green'),
             'fruit': _gc('LightMagenta'),
         }
 
-        def __init__(self, value: _Union[str, int], children: list = None, indent: int = 4,
-                     colors: _Mapping[str, str] = None, mode='-'):
+        def __init__(self, value: _Union[str, int], children: _Optional[_List[TreePrint.Node]] = None, indent: int = 4,
+                     colors: _Optional[_Mapping[str, str]] = None, mode: str='-'):
             self.value = str(value)
             if children:
                 self._children = children
             else:
                 self._children = []
             self.indent = indent
             self.colors = self.colors.copy()
@@ -29,24 +31,25 @@
             if not mode:
                 self.mode = 1
             else:
                 self.mode = self._get_mode(mode)
                 if self.mode == -1:
                     raise ValueError('`mode` must be - or =')
 
-        def _get_mode(self, mode=None) -> int:
+        def _get_mode(self, mode: _Optional[_Union[str, int]] = None) -> int:
             if not mode:
                 mode = self.mode
             if isinstance(mode, int):
                 if mode in [1, 2]:
                     return mode
-            if mode in '-_─┌│|└┬├└':
-                return 1
-            if mode in '=═╔║╠╚╦╚':
-                return 2
+            elif isinstance(mode, str):
+                if mode in '-_─┌│|└┬├└':
+                    return 1
+                if mode in '=═╔║╠╚╦╚':
+                    return 2
             return -1
 
         def __str__(self, level=0, prefix='', mode=None):
             mode = self._get_mode(mode)
             if mode == -1:
                 raise ValueError('`mode` must be - or =')
             chars = '─┌│└┬├└'
@@ -84,34 +87,34 @@
                 text += child.__str__(level=level + 1, prefix=prefix_, mode=mode)
 
             return text
 
         def has_child(self):
             return len(self._children) > 0
 
-        def add_child(self, child: 'TreePrint.Node'):
+        def add_child(self, child: TreePrint.Node):
             if not isinstance(child, TreePrint.Node):
                 raise TypeError('`child` must be TreePrint.Node')
             self._children.append(child)
 
-        def get_child(self, value: str = None, index: int = None):
+        def get_child(self, value: _Optional[str] = None, index: _Optional[int] = None):
             if value and index:
                 raise ValueError('`value` and `index` can not be both set')
             if not value and not index:
                 raise ValueError('`value` or `index` must be set')
             if value:
                 for child in self._children:
                     if child.value == value:
                         return child
             if index:
                 return self._children[index]
 
         @staticmethod
-        def add_to(node: 'TreePrint.Node', data: _Union[_Mapping, _Sequence, str, int], indent: int = 4,
-                   colors: _Mapping[str, str] = None, mode='-'):
+        def add_to(node: TreePrint.Node, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4,
+                   colors: _Optional[_Mapping[str, str]] = None, mode='-'):
             if isinstance(data, _Mapping):
                 if len(data) == 1:
                     child = TreePrint.Node(list(data.keys())[0], indent=indent, colors=colors, mode=mode)
                     TreePrint.Node.add_to(child, list(data.values())[0], indent=indent, colors=colors, mode=mode)
                     node.add_child(child)
                 else:
                     for key, value in data.items():
@@ -133,15 +136,15 @@
                         child = TreePrint.Node(str(value), indent=indent, colors=colors, mode=mode)
                         node.add_child(child)
             else:
                 child = TreePrint.Node(str(data), indent=indent, colors=colors, mode=mode)
                 node.add_child(child)
 
     def __init__(self, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, 
-                 colors: _Mapping[str, str] = None, mode='-'):
+                 colors: _Optional[_Mapping[str, str]] = None, mode='-'):
         self.indent = indent
         self.mode = mode
         if isinstance(data, _Mapping):
             if len(data) == 1:
                 self.root = self.Node(list(data.keys())[0], indent=indent, colors=colors)
                 self.add_to_root(list(data.values()), colors=colors)
             else:
@@ -149,19 +152,19 @@
                 self.add_to_root(data, colors=colors)
         elif isinstance(data, _Sequence):
             self.root = self.Node('root', indent=indent, colors=colors)
             self.add_to_root(data, colors=colors)
         else:
             self.root = self.Node(str(data), indent=indent, colors=colors)
 
-    def add_to_root(self, data: _Union[_Mapping, _Sequence, str, int], colors: _Mapping[str, str] = None):
+    def add_to_root(self, data: _Union[_Mapping, _Sequence, str, int], colors: _Optional[_Mapping[str, str]] = None):
         self.Node.add_to(self.root, data, indent=self.indent, colors=colors, mode=self.mode)
 
     def __str__(self, mode=None):
         if not mode:
             mode = self.mode
         return self.root.__str__(mode=mode)
 
 
 def tree_format(data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, mode='-',
-                colors: _Mapping[str, str] = None):
+                colors: _Optional[_Mapping[str, str]] = None):
     return str(TreePrint(data, indent=indent, colors=colors, mode=mode))
```

### Comparing `log21-2.5.1/log21/__init__.py` & `log21-2.5.2/log21/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # log21.__init__.py
 # CodeWriter21
 
 import io as _io
 import os as _os
 import logging as _logging
 
-from typing import Union as _Union, Mapping as _Mapping, Type as _Type, Tuple as _Tuple
+from typing import Union as _Union, Mapping as _Mapping, Type as _Type, Tuple as _Tuple, Optional as _Optional
 
 import log21.CrashReporter as CrashReporter
 
 from log21.Levels import INPUT, CRITICAL, FATAL, ERROR, WARNING, WARN, INFO, DEBUG, NOTSET
 from log21.Logger import Logger
 from log21.Manager import Manager
 from log21.ProgressBar import ProgressBar
@@ -18,48 +18,48 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.5.1"
+__version__ = "2.5.2"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
-           'INFO', 'DEBUG', 'NOTSET', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
+           'INFO', 'DEBUG', 'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
            'critical', 'fatal', 'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
            'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter', 'console_reporter',
            'file_reporter']
 
 _manager = Manager()
 _logging.setLoggerClass(Logger)
 
 
-def _prepare_formatter(fmt: str = None, style: str = '%', datefmt: str = "%H:%M:%S", show_level: bool = True,
-                       show_time: bool = True, colorize_time_and_level: bool = True,
-                       level_names: _Mapping[int, str] = None, 
-                       level_colors: _Mapping[int, _Tuple[str, ...]] = None,
+def _prepare_formatter(fmt: _Optional[str] = None, style: str = '%', datefmt: str = "%H:%M:%S",
+                       show_level: bool = True, show_time: bool = True, colorize_time_and_level: bool = True,
+                       level_names: _Optional[_Mapping[int, str]] = None,
+                       level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
                        formatter_class: _Type[_logging.Formatter] = ColorizingFormatter):
     # Prepares a formatting if the fmt was None
     if not fmt:
         style = '%'
         fmt = "%(message)s"
         if show_level:
             fmt = "[%(levelname)s] " + fmt
         if show_time:
             fmt = "[%(asctime)s] " + fmt
         fmt = '\r' + fmt
 
     if level_colors and not issubclass(formatter_class, ColorizingFormatter):
         warning('`formatter_class` should be a subclass of ColorizingFormatter when used with level_colors.')
-        warning(f'Using `{formatter_class.__class__.__name__}` might lead to unexpected behaviour!')
+        warning(f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!')
 
     # Defines the formatter
     if level_colors:
         formatter = formatter_class(fmt, datefmt, style=style, level_colors=level_colors)
     else:
         formatter = formatter_class(fmt, datefmt, style=style)
     
@@ -70,19 +70,19 @@
             formatter.level_colors[key] = tuple()
         formatter.time_color = tuple()
 
     return formatter
 
 
 def get_logger(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
-               show_level: bool = True, colorize_time_and_level: bool = True, fmt: str = None,
+               show_level: bool = True, colorize_time_and_level: bool = True, fmt: _Optional[str] = None,
                datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-               handle_new_line: bool = True, override=False, level_names: _Mapping[int, str] = None,
-               level_colors: _Mapping[int, _Tuple[str, ...]] = None,
-               file: _Union[_os.PathLike, str] = None) -> Logger:
+               handle_new_line: bool = True, override=False, level_names: _Optional[_Mapping[int, str]] = None,
+               level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+               file: _Optional[_Union[_os.PathLike, str]] = None) -> _Union[Logger, _logging.Logger]:
     """
     Returns a logging.Logger with colorizing support.
     >>>
     >>> import log21
     >>>
     >>> l = log21.get_logger()
     >>> l.warning('Pretty basic, huh?')
@@ -165,17 +165,17 @@
             file_handler.setFormatter(file_formatter)
             logger.addHandler(file_handler)
 
     return logger
 
 
 def get_logging_window(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
-                       show_level: bool = True, colorize_time_and_level: bool = True, fmt: str = None,
+                       show_level: bool = True, colorize_time_and_level: bool = True, fmt: _Optional[str] = None,
                        datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-                       handle_new_line: bool = True, override=False, level_names: _Mapping[int, str] = None,
+                       handle_new_line: bool = True, override=False, level_names: _Optional[_Mapping[int, str]] = None,
                        width: int = 80, height: int = 20, allow_shell: bool = False) -> LoggingWindow:
     """
     Returns a logging window.
 
     >>> # Let's see how it works
     >>> # Imports log21 and time modules
     >>> import log21, time
@@ -258,15 +258,15 @@
 
 
 def getpass(*msg, args: tuple = (), end='', **kwargs):
     logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
     return logger.getpass(*msg, args=args, end=end, **kwargs)
 
 
-def pprint(obj, indent=1, width=80, depth=None, signs_colors: _Mapping[str, str] = None, *, sort_dicts=True,
+def pprint(obj, indent=1, width=80, depth=None, signs_colors: _Optional[_Mapping[str, str]] = None, *, sort_dicts=True,
            underscore_numbers=False, compact=False, end='\033[0m\n', **kwargs):
     logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
     logger.print(pformat(obj=obj, indent=indent, width=width, depth=depth, signs_colors=signs_colors, compact=compact,
                          sort_dicts=sort_dicts, underscore_numbers=underscore_numbers), end=end, **kwargs)
 
 
 pretty_print = pprint
@@ -278,15 +278,15 @@
 
 
 tprint = tree_print
 
 root = Logger('root-logger', INFO)
 
 
-def basic_config(force: bool = False, encoding: str = None, errors: str = 'backslashreplace', handlers=None,
+def basic_config(force: bool = False, encoding: str = None, errors: _Optional[str] = 'backslashreplace', handlers=None,
                  stream=None, filename=None, filemode: str = 'a', date_format: str = "%H:%M:%S", style: str = '%',
                  format_: str = None, level: _Union[int, str] = None):
     """
     Do basic configuration for the logging system.
 
     This function does nothing if the root logger already has handlers
     configured, unless the keyword argument *force* is set to ``True``.
@@ -452,15 +452,15 @@
     basicConfig() to add a console handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.log(level, *msg, args=args, **kwargs)
 
 
-def progress_bar(progress: float, total: float, width: int = None, prefix: str = '|', suffix: str = '|',
+def progress_bar(progress: float, total: float, width: _Optional[int] = None, prefix: str = '|', suffix: str = '|',
                  show_percentage: bool = True):
     """
     Print a progress bar to the console.
     """
 
     bar = ProgressBar(width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage)
```

### Comparing `log21-2.5.1/log21.egg-info/PKG-INFO` & `log21-2.5.2/log21.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.1
+Version: 2.5.2
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
@@ -71,17 +71,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.1
+### 2.5.2
 
-Switched from `setup.py` build system to `pyproject.toml`
+Improved type-hintings.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.1/log21.egg-info/SOURCES.txt` & `log21-2.5.2/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.1/pyproject.toml` & `log21-2.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "log21"
 authors = [
   {name = "CodeWriter21(Mehrad Pooryoussof)", email = "CodeWriter21@gmail.com"}
 ]
 description = "A simple logging package that helps you log colorized messages in Windows console."
 readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 keywords = ['python', 'log', 'colorize', 'color', 'logging', 'Python3', 'CodeWriter21']
 license = {text = "Apache License 2.0"}
 classifiers = [
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.10",
@@ -21,13 +21,13 @@
   "Operating System :: Unix",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
   "webcolors"
 ]
-version = "2.5.1"
+version = "2.5.2"
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
 Source = "https://github.com/MPCodeWriter21/log21"
```

