# Comparing `tmp/log21-2.5.2.tar.gz` & `tmp/log21-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.5.2.tar", last modified: Tue Jun 27 02:58:12 2023, max compression
+gzip compressed data, was "log21-2.5.3.tar", last modified: Tue Jun 27 11:02:07 2023, max compression
```

## Comparing `log21-2.5.2.tar` & `log21-2.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-27 02:58:02.000000 log21-2.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-27 02:58:12.259999 log21-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-27 02:58:02.000000 log21-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21666 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 02:58:02.000000 log21-2.5.2/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-27 02:58:02.000000 log21-2.5.2/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-27 02:58:02.000000 log21-2.5.2/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 02:58:02.000000 log21-2.5.2/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-06-27 02:58:02.000000 log21-2.5.2/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 02:58:02.000000 log21-2.5.2/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-06-27 02:58:02.000000 log21-2.5.2/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-27 02:58:02.000000 log21-2.5.2/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-27 02:58:02.000000 log21-2.5.2/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-27 02:58:02.000000 log21-2.5.2/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-27 02:58:02.000000 log21-2.5.2/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:58:12.259999 log21-2.5.2/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 02:58:12.000000 log21-2.5.2/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-27 02:58:02.000000 log21-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 02:58:12.259999 log21-2.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-27 11:01:57.000000 log21-2.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-27 11:02:07.733104 log21-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-27 11:01:57.000000 log21-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 11:01:57.000000 log21-2.5.3/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-27 11:01:57.000000 log21-2.5.3/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-27 11:01:57.000000 log21-2.5.3/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 11:01:57.000000 log21-2.5.3/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-06-27 11:01:57.000000 log21-2.5.3/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-06-27 11:01:57.000000 log21-2.5.3/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-27 11:01:57.000000 log21-2.5.3/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-27 11:01:57.000000 log21-2.5.3/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-06-27 11:01:57.000000 log21-2.5.3/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-27 11:01:57.000000 log21-2.5.3/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-27 11:01:57.000000 log21-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:02:07.733104 log21-2.5.3/setup.cfg
```

### Comparing `log21-2.5.2/LICENSE.txt` & `log21-2.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/PKG-INFO` & `log21-2.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: log21
-Version: 2.5.2
-Summary: A simple logging package that helps you log colorized messages in Windows console.
-Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
-License: Apache License 2.0
-Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
-Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
-Project-URL: Source, https://github.com/MPCodeWriter21/log21
-Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/log21)
 ![forks](https://img.shields.io/github/forks/MPCodeWriter21/log21)
 ![repo size](https://img.shields.io/github/repo-size/MPCodeWriter21/log21)
@@ -71,17 +49,21 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.2
+### 2.5.3
 
-Improved type-hintings.
+Moved some dictionaries to `__init__` methods.
+`colors` in `Argparse.ColorizingHelpFormatter` class.
+`_level_name` in `Formatters._Formatter` class and `level_colors` in `Formatters.ColorizingFormatter` class.
+`sign_colors` in `PPrint.PrettyPrinter` class.
+`colors` in `TreePrint.TreePrint.Node` class.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.2/README.md` & `log21-2.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: log21
+Version: 2.5.3
+Summary: A simple logging package that helps you log colorized messages in Windows console.
+Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
+Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
+Project-URL: Source, https://github.com/MPCodeWriter21/log21
+Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/log21)
 ![forks](https://img.shields.io/github/forks/MPCodeWriter21/log21)
 ![repo size](https://img.shields.io/github/repo-size/MPCodeWriter21/log21)
@@ -49,17 +71,21 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.2
+### 2.5.3
 
-Improved type-hintings.
+Moved some dictionaries to `__init__` methods.
+`colors` in `Argparse.ColorizingHelpFormatter` class.
+`_level_name` in `Formatters._Formatter` class and `level_colors` in `Formatters.ColorizingFormatter` class.
+`sign_colors` in `PPrint.PrettyPrinter` class.
+`colors` in `TreePrint.TreePrint.Node` class.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.2/log21/Argparse.py` & `log21-2.5.3/log21/Argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 from log21.Colors import get_colors as _gc
 from log21.Formatters import DecolorizingFormatter as _Formatter
 
 __all__ = ['ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper']
 
 
 class ColorizingHelpFormatter(_argparse.HelpFormatter):
-    colors = {
-        'usage': 'Cyan',
-        'brackets': 'LightRed',
-        'switches': 'LightCyan',
-        'values': 'Green',
-        'colons': 'LightRed',
-        'commas': 'LightRed',
-        'section headers': 'LightGreen',
-        'help': 'LightWhite',
-        'choices': 'LightGreen'
-    }
-
-    def __init__(self, prog, indent_increment=2, max_help_position=24, width=None, colors: _Mapping[str, str] = None):
+    def __init__(self, prog, indent_increment=2, max_help_position=24, width=None,
+                 colors: _Optional[_Mapping[str, str]] = None):
         super().__init__(prog, indent_increment, max_help_position, width)
+        
+        self.colors = {
+            'usage': 'Cyan',
+            'brackets': 'LightRed',
+            'switches': 'LightCyan',
+            'values': 'Green',
+            'colons': 'LightRed',
+            'commas': 'LightRed',
+            'section headers': 'LightGreen',
+            'help': 'LightWhite',
+            'choices': 'LightGreen'
+        }
+
         if colors:
             for key, value in colors.items():
                 if key in self.colors:
                     self.colors[key] = value
 
     class _Section(object):
         def __init__(self, formatter, parent, heading=None):
```

### Comparing `log21-2.5.2/log21/Colors.py` & `log21-2.5.3/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/CrashReporter/Formatters.py` & `log21-2.5.3/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/CrashReporter/Reporters.py` & `log21-2.5.3/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/FileHandler.py` & `log21-2.5.3/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/Formatters.py` & `log21-2.5.3/log21/Formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,14 @@
 from log21.Colors import get_colors as _gc, ansi_escape
 from log21.Levels import INPUT, CRITICAL, ERROR, WARNING, INFO, DEBUG, PRINT
 
 __all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
 
 
 class _Formatter(__Formatter):
-    _level_names: _Dict[int, str] = {
-        DEBUG: 'DEBUG',
-        INFO: 'INFO',
-        WARNING: 'WARNING',
-        ERROR: 'ERROR',
-        CRITICAL: 'CRITICAL',
-        PRINT: 'PRINT',
-        INPUT: 'INPUT'
-    }
-
     def __init__(self, fmt: _Optional[str] = None, datefmt: _Optional[str] = None, style: str = '%',
                  level_names: _Optional[_Mapping[int, str]] = None):
         """
         `level_names` usage:
         >>> import log21
         >>> logger = log21.Logger('MyLogger', log21.DEBUG)
         >>> stream_handler = log21.ColorizingStreamHandler()
@@ -45,14 +35,25 @@
         >>> logger.critical('Crashed....')
         [X] Crashed....
         >>>
         >>> # Hope you've enjoyed
         >>>
         """
         super().__init__(fmt=fmt, datefmt=datefmt, style=style)
+
+        self._level_names: _Dict[int, str] = {
+            DEBUG: 'DEBUG',
+            INFO: 'INFO',
+            WARNING: 'WARNING',
+            ERROR: 'ERROR',
+            CRITICAL: 'CRITICAL',
+            PRINT: 'PRINT',
+            INPUT: 'INPUT'
+        }
+
         if level_names:
             for level, name in level_names.items():
                 self.level_names[level] = name
 
     @property
     def level_names(self):
         return self._level_names
@@ -85,37 +86,36 @@
             if s[-1:] != "\n":
                 s = s + "\n"
             s = s + self.formatStack(record.stack_info)
         return s
 
 
 class ColorizingFormatter(_Formatter):
-    # Default color values
-    level_colors: _Dict[int, _Tuple[str, ...]] = {
-        DEBUG: ('lightblue',),
-        INFO: ('green',),
-        WARNING: ('lightyellow',),
-        ERROR: ('light red',),
-        CRITICAL: ('background red', 'white'),
-        PRINT: ('Cyan',),
-        INPUT: ('Magenta',)
-    }
     time_color: _Tuple[str, ...] = ('lightblue',)
     name_color = pathname_color = filename_color = module_color = func_name_color = thread_name_color = \
         message_color = tuple()
 
     def __init__(self, fmt: _Optional[str] = None, datefmt: _Optional[str] = None, style: str = '%',
                  level_names: _Optional[_Mapping[int, str]] = None,
                  level_colors: _Optional[_Mapping[int, _Tuple[str]]] = None,
                  time_color: _Optional[_Tuple[str, ...]] = None, name_color: _Optional[_Tuple[str, ...]] = None,
                  pathname_color: _Optional[_Tuple[str, ...]] = None, filename_color: _Optional[_Tuple[str, ...]] = None,
                  module_color: _Optional[_Tuple[str, ...]] = None, func_name_color: _Optional[_Tuple[str, ...]] = None,
                  thread_name_color: _Optional[_Tuple[str, ...]] = None,
                  message_color: _Optional[_Tuple[str, ...]] = None):
         super().__init__(fmt=fmt, datefmt=datefmt, style=style, level_names=level_names)
+        self.level_colors: _Dict[int, _Tuple[str, ...]] = {
+            DEBUG: ('lightblue',),
+            INFO: ('green',),
+            WARNING: ('lightyellow',),
+            ERROR: ('light red',),
+            CRITICAL: ('background red', 'white'),
+            PRINT: ('Cyan',),
+            INPUT: ('Magenta',)
+        }
         # Checks and sets colors
         if level_colors:
             if not isinstance(level_colors, _Mapping):
                 raise TypeError('`level_colors` must be a dictionary like object!')
             for level, color in level_colors.items():
                 self.level_colors[level] = (_gc(*color),)
         if time_color:
```

### Comparing `log21-2.5.2/log21/Logger.py` & `log21-2.5.3/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/LoggingWindow.py` & `log21-2.5.3/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/Manager.py` & `log21-2.5.3/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/PPrint.py` & `log21-2.5.3/log21/PPrint.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re as _re
 import sys as _sys
 import types as _types
 import collections as _collections
 import dataclasses as _dataclasses
 
 from pprint import PrettyPrinter as _PrettyPrinter
-from typing import Mapping as _Mapping, Optional as _Optional
+from typing import Mapping as _Mapping, Optional as _Optional, Dict as _Dict
 
 from log21.Colors import get_colors as _gc
 
 _builtin_scalars = frozenset({str, bytes, bytearray, float, complex, bool, type(None)})
 
 
 def _recursion(obj):
@@ -61,40 +61,40 @@
         try:
             return self.obj < other.obj
         except TypeError:
             return (str(type(self.obj)), id(self.obj)) < (str(type(other.obj)), id(other.obj))
 
 
 class PrettyPrinter(_PrettyPrinter):
-    signs_colors: _Mapping[str, str] = {
-        'square-brackets': _gc('LightCyan'),
-        'curly-braces': _gc('LightBlue'),
-        'parenthesis': _gc('LightGreen'),
-        'comma': _gc('LightRed'),
-        'colon': _gc('LightRed'),
-        '...': _gc('LightMagenta'),
-        'data': _gc('Green')
-    }
-
-    def __init__(self, indent=1, width=80, depth=None, stream=None, signs_colors: _Optional[_Mapping[str, str]] = None,
+    def __init__(self, indent=1, width=80, depth=None, stream=None, sign_colors: _Optional[_Mapping[str, str]] = None,
                  *, compact=False, sort_dicts=True, underscore_numbers=False, **kwargs):
         super().__init__(indent=indent, width=width, depth=depth, stream=stream, compact=compact, **kwargs)
         self._depth = depth
         self._indent_per_level = indent
         self._width = width
         if stream is not None:
             self._stream = stream
         else:
             self._stream = _sys.stdout
         self._compact = bool(compact)
         self._sort_dicts = sort_dicts
         self._underscore_numbers = underscore_numbers
-        if signs_colors:
-            for sign, color in signs_colors.items():
-                self.signs_colors[sign.lower()] = _gc(color)
+
+        self.sign_colors: _Dict[str, str] = {
+            'square-brackets': _gc('LightCyan'),
+            'curly-braces': _gc('LightBlue'),
+            'parenthesis': _gc('LightGreen'),
+            'comma': _gc('LightRed'),
+            'colon': _gc('LightRed'),
+            '...': _gc('LightMagenta'),
+            'data': _gc('Green')
+        }
+        if sign_colors:
+            for sign, color in sign_colors.items():
+                self.sign_colors[sign.lower()] = _gc(color)
 
     def _format(self, obj, stream, indent, allowance, context, level):
         objid = id(obj)
         if objid in context:
             stream.write(_recursion(obj))
             self._recursive = True
             self._readable = False
@@ -149,19 +149,19 @@
             if self._underscore_numbers:
                 return f"{object_:_d}", True, False
             else:
                 return repr(object_), True, False
 
         if issubclass(type_, dict) and representation is dict.__repr__:
             if not object_:
-                return self.signs_colors.get('curly-braces') + "{}" + self.signs_colors.get('data'), True, False
+                return self.sign_colors.get('curly-braces') + "{}" + self.sign_colors.get('data'), True, False
             object_id = id(object_)
             if max_levels and level >= max_levels:
-                return self.signs_colors.get('curly-braces') + "{" + self.signs_colors.get('...') + "..." + \
-                       self.signs_colors.get('curly-braces') + "}" + self.signs_colors.get('data'), \
+                return self.sign_colors.get('curly-braces') + "{" + self.sign_colors.get('...') + "..." + \
+                       self.sign_colors.get('curly-braces') + "}" + self.sign_colors.get('data'), \
                        False, object_id in context
             if object_id in context:
                 return _recursion(object_), False, True
             context[object_id] = 1
             readable = True
             recursive = False
             components = []
@@ -170,42 +170,42 @@
             if self._sort_dicts:
                 items = sorted(object_.items(), key=_safe_tuple)
             else:
                 items = object_.items()
             for k, v in items:
                 krepr, kreadable, krecur = self.format(k, context, max_levels, level)
                 vrepr, vreadable, vrecur = self.format(v, context, max_levels, level)
-                append(f"{krepr}{self.signs_colors.get('colon')}:{self.signs_colors.get('data')} {vrepr}")
+                append(f"{krepr}{self.sign_colors.get('colon')}:{self.sign_colors.get('data')} {vrepr}")
                 readable = readable and kreadable and vreadable
                 if krecur or vrecur:
                     recursive = True
             del context[object_id]
-            return self.signs_colors.get('curly-braces') + "{" + self.signs_colors.get('data') + \
-                   (self.signs_colors.get('comma') + ", " + self.signs_colors.get('data')).join(components) + \
-                   self.signs_colors.get('curly-braces') + "}", readable, recursive
+            return self.sign_colors.get('curly-braces') + "{" + self.sign_colors.get('data') + \
+                   (self.sign_colors.get('comma') + ", " + self.sign_colors.get('data')).join(components) + \
+                   self.sign_colors.get('curly-braces') + "}", readable, recursive
 
         if (issubclass(type_, list) and representation is list.__repr__) or \
                 (issubclass(type_, tuple) and representation is tuple.__repr__):
             if issubclass(type_, list):
                 if not object_:
-                    return self.signs_colors.get('square-brackets') + "[]" + self.signs_colors.get('data'), True, False
-                format_ = self.signs_colors.get('square-brackets') + "[" + self.signs_colors.get('data') + "%s" + \
-                          self.signs_colors.get('square-brackets') + "]" + self.signs_colors.get('data')
+                    return self.sign_colors.get('square-brackets') + "[]" + self.sign_colors.get('data'), True, False
+                format_ = self.sign_colors.get('square-brackets') + "[" + self.sign_colors.get('data') + "%s" + \
+                          self.sign_colors.get('square-brackets') + "]" + self.sign_colors.get('data')
             elif len(object_) == 1:
-                format_ = self.signs_colors.get('parenthesis') + "(" + self.signs_colors.get('data') + "%s" + \
-                          self.signs_colors.get('comma') + "," + self.signs_colors.get('parenthesis') + ")" + \
-                          self.signs_colors.get('data')
+                format_ = self.sign_colors.get('parenthesis') + "(" + self.sign_colors.get('data') + "%s" + \
+                          self.sign_colors.get('comma') + "," + self.sign_colors.get('parenthesis') + ")" + \
+                          self.sign_colors.get('data')
             else:
                 if not object_:
-                    return self.signs_colors.get('parenthesis') + "()" + self.signs_colors.get('data'), True, False
-                format_ = self.signs_colors.get('parenthesis') + "(" + self.signs_colors.get('data') + "%s" + \
-                          self.signs_colors.get('parenthesis') + ")" + self.signs_colors.get('data')
+                    return self.sign_colors.get('parenthesis') + "()" + self.sign_colors.get('data'), True, False
+                format_ = self.sign_colors.get('parenthesis') + "(" + self.sign_colors.get('data') + "%s" + \
+                          self.sign_colors.get('parenthesis') + ")" + self.sign_colors.get('data')
             object_id = id(object_)
             if max_levels and level >= max_levels:
-                return format_ % self.signs_colors.get('...') + "...", False, object_id in context
+                return format_ % self.sign_colors.get('...') + "...", False, object_id in context
             if object_id in context:
                 return _recursion(object_), False, True
             context[object_id] = 1
             readable = True
             recursive = False
             components = []
             append = components.append
@@ -214,84 +214,84 @@
                 orepr, oreadable, orecur = self.format(o, context, max_levels, level)
                 append(orepr)
                 if not oreadable:
                     readable = False
                 if orecur:
                     recursive = True
             del context[object_id]
-            return format_ % (self.signs_colors.get('comma') + ", " + self.signs_colors.get('data')).join(components), \
+            return format_ % (self.sign_colors.get('comma') + ", " + self.sign_colors.get('data')).join(components), \
                    readable, recursive
 
         rep = repr(object_)
         return rep, (rep and not rep.startswith('<')), False
 
     _dispatch = {}
 
     def _pprint_dict(self, obj, stream, indent, allowance, context, level):
         write = stream.write
-        write(self.signs_colors.get('curly-braces') + '{' + self.signs_colors.get('data'))
+        write(self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
         if self._indent_per_level > 1:
             write((self._indent_per_level - 1) * ' ')
         length = len(obj)
         if length:
             if self._sort_dicts:
                 items = sorted(obj.items(), key=_safe_tuple)
             else:
                 items = obj.items()
             self._format_dict_items(items, stream, indent, allowance + 1,
                                     context, level)
-        write(self.signs_colors.get('curly-braces') + '}' + self.signs_colors.get('data'))
+        write(self.sign_colors.get('curly-braces') + '}' + self.sign_colors.get('data'))
 
     _dispatch[dict.__repr__] = _pprint_dict
 
     def _pprint_ordered_dict(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         self._format(list(obj.items()), stream,
                      indent + len(cls.__name__) + 1, allowance + 1,
                      context, level)
-        stream.write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[_collections.OrderedDict.__repr__] = _pprint_ordered_dict
 
     def _pprint_list(self, obj, stream, indent, allowance, context, level):
-        stream.write(self.signs_colors.get('square-brackets') + '[' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('square-brackets') + '[' + self.sign_colors.get('data'))
         self._format_items(obj, stream, indent, allowance + 1,
                            context, level)
-        stream.write(self.signs_colors.get('square-brackets') + ']' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('square-brackets') + ']' + self.sign_colors.get('data'))
 
     _dispatch[list.__repr__] = _pprint_list
 
     def _pprint_tuple(self, obj, stream, indent, allowance, context, level):
-        stream.write(self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
-        endchar = self.signs_colors.get('comma') + ',' + self.signs_colors.get('parenthesis') + ')' + \
-                  self.signs_colors.get('data') if len(obj) == 1 else self.signs_colors.get('parenthesis') + ')' + \
-                                                                      self.signs_colors.get('data')
+        stream.write(self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+        endchar = self.sign_colors.get('comma') + ',' + self.sign_colors.get('parenthesis') + ')' + \
+                  self.sign_colors.get('data') if len(obj) == 1 else self.sign_colors.get('parenthesis') + ')' + \
+                                                                      self.sign_colors.get('data')
         self._format_items(obj, stream, indent, allowance + len(endchar),
                            context, level)
         stream.write(endchar)
 
     _dispatch[tuple.__repr__] = _pprint_tuple
 
     def _pprint_set(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         typ = obj.__class__
         if typ is set:
-            stream.write(self.signs_colors.get('curly-braces') + '{' + self.signs_colors.get('data'))
-            endchar = self.signs_colors.get('curly-braces') + '}' + self.signs_colors.get('data')
+            stream.write(self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
+            endchar = self.sign_colors.get('curly-braces') + '}' + self.sign_colors.get('data')
         else:
-            stream.write(typ.__name__ + self.signs_colors.get('parenthesis') + '(' +
-                         self.signs_colors.get('curly-braces') + '{' + self.signs_colors.get('data'))
-            endchar = self.signs_colors.get('curly-braces') + '}' + self.signs_colors.get('parenthesis') + ')' \
-                      + self.signs_colors.get('data')
+            stream.write(typ.__name__ + self.sign_colors.get('parenthesis') + '(' +
+                         self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
+            endchar = self.sign_colors.get('curly-braces') + '}' + self.sign_colors.get('parenthesis') + ')' \
+                      + self.sign_colors.get('data')
             indent += len(typ.__name__) + 1
         obj = sorted(obj, key=_SafeKey)
         self._format_items(obj, stream, indent, allowance + len(endchar),
                            context, level)
         stream.write(endchar)
 
     _dispatch[set.__repr__] = _pprint_set
@@ -335,116 +335,116 @@
                         current = candidate
                 if current:
                     chunks.append(repr(current))
         if len(chunks) == 1:
             write(representation)
             return
         if level == 1:
-            write(self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+            write(self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         for i, representation in enumerate(chunks):
             if i > 0:
                 write('\n' + ' ' * indent)
             write(representation)
         if level == 1:
-            write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+            write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[str.__repr__] = _pprint_str
 
     def _pprint_bytes(self, obj, stream, indent, allowance, context, level):
         write = stream.write
         if len(obj) <= 4:
             write(repr(obj))
             return
         parens = level == 1
         if parens:
             indent += 1
             allowance += 1
-            write(self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+            write(self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         delim = ''
         for rep in _wrap_bytes_repr(obj, self._width - indent, allowance):
             write(delim)
             write(rep)
             if not delim:
                 delim = '\n' + ' ' * indent
         if parens:
-            write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+            write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[bytes.__repr__] = _pprint_bytes
 
     def _pprint_bytearray(self, obj, stream, indent, allowance, context, level):
         write = stream.write
-        write('bytearray' + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+        write('bytearray' + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         self._pprint_bytes(bytes(obj), stream, indent + 10,
                            allowance + 1, context, level + 1)
-        write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+        write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[bytearray.__repr__] = _pprint_bytearray
 
     def _pprint_mappingproxy(self, obj, stream, indent, allowance, context, level):
-        stream.write('mappingproxy' + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+        stream.write('mappingproxy' + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         self._format(obj.copy(), stream, indent + 13, allowance + 1,
                      context, level)
-        stream.write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[_types.MappingProxyType.__repr__] = _pprint_mappingproxy
 
     def _pprint_simplenamespace(self, obj, stream, indent, allowance, context, level):
         if type(obj) is _types.SimpleNamespace:
             # The SimpleNamespace repr is "namespace" instead of the class
             # name, so we do the same here. For subclasses; use the class name.
             cls_name = 'namespace'
         else:
             cls_name = obj.__class__.__name__
         indent += len(cls_name) + 1
         items = obj.__dict__.items()
-        stream.write(cls_name + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+        stream.write(cls_name + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         self._format_namespace_items(items, stream, indent, allowance, context, level)
-        stream.write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[_types.SimpleNamespace.__repr__] = _pprint_simplenamespace
 
     def _format_dict_items(self, items, stream, indent, allowance, context, level):
         write = stream.write
         indent += self._indent_per_level
-        delimnl = self.signs_colors.get('comma') + ',\n' + self.signs_colors.get('data') + ' ' * indent
+        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent
         last_index = len(items) - 1
         for i, (key, ent) in enumerate(items):
             last = i == last_index
             rep = self._repr(key, context, level)
             write(rep)
-            write(self.signs_colors.get('colon') + ': ' + self.signs_colors.get('data'))
+            write(self.sign_colors.get('colon') + ': ' + self.sign_colors.get('data'))
             self._format(ent, stream, indent + len(rep) + 2,
                          allowance if last else 1,
                          context, level)
             if not last:
                 write(delimnl)
 
     def _format_namespace_items(self, items, stream, indent, allowance, context, level):
         write = stream.write
-        delimnl = self.signs_colors.get('comma') + ',\n' + self.signs_colors.get('data') + ' ' * indent
+        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent
         last_index = len(items) - 1
         for i, (key, ent) in enumerate(items):
             last = i == last_index
             write(key)
             write('=')
             if id(ent) in context:
                 # Special-case representation of recursion to match standard
                 # recursive dataclass repr.
-                write(self.signs_colors.get('...') + "..." + self.signs_colors.get('data'))
+                write(self.sign_colors.get('...') + "..." + self.sign_colors.get('data'))
             else:
                 self._format(ent, stream, indent + len(key) + 1, allowance if last else 1, context, level)
             if not last:
                 write(delimnl)
 
     def _format_items(self, items, stream, indent, allowance, context, level):
         write = stream.write
         indent += self._indent_per_level
         if self._indent_per_level > 1:
             write((self._indent_per_level - 1) * ' ')
-        delimnl = self.signs_colors.get('comma') + ',\n' + self.signs_colors.get('data') + ' ' * indent
+        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent
         delim = ''
         width = max_width = self._width - indent + 1
         it = iter(items)
         try:
             next_ent = next(it)
         except StopIteration:
             return
@@ -463,90 +463,90 @@
                 if width < w:
                     width = max_width
                     if delim:
                         delim = delimnl
                 if width >= w:
                     width -= w
                     write(delim)
-                    delim = self.signs_colors.get('comma') + ', ' + self.signs_colors.get('data')
+                    delim = self.sign_colors.get('comma') + ', ' + self.sign_colors.get('data')
                     write(rep)
                     continue
             write(delim)
             delim = delimnl
             self._format(ent, stream, indent, allowance if last else 1, context, level)
 
     def _pprint_default_dict(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         rdf = self._repr(obj.default_factory, context, level)
         cls = obj.__class__
         indent += len(cls.__name__) + 1
-        stream.write(cls.__name__ + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data') + rdf +
-                     self.signs_colors.get('comma') + ',\n' + self.signs_colors.get('data') + (' ' * indent))
+        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data') + rdf +
+                     self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + (' ' * indent))
         self._pprint_dict(obj, stream, indent, allowance + 1, context, level)
-        stream.write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[_collections.defaultdict.__repr__] = _pprint_default_dict
 
     def _pprint_counter(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.signs_colors.get('parenthesis') + '(' +
-                     self.signs_colors.get('curly-braces') + '{' + self.signs_colors.get('data'))
+        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+                     self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
         if self._indent_per_level > 1:
             stream.write((self._indent_per_level - 1) * ' ')
         items = obj.most_common()
         self._format_dict_items(items, stream,
                                 indent + len(cls.__name__) + 1, allowance + 2,
                                 context, level)
-        stream.write(self.signs_colors.get('curly-braces') + '}' +
-                     self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('curly-braces') + '}' +
+                     self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[_collections.Counter.__repr__] = _pprint_counter
 
     def _pprint_chain_map(self, obj, stream, indent, allowance, context, level):
         if not len(obj.maps):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         indent += len(cls.__name__) + 1
         for i, m in enumerate(obj.maps):
             if i == len(obj.maps) - 1:
                 self._format(m, stream, indent, allowance + 1, context, level)
-                stream.write(self.signs_colors.get('parenthesis') + ')' + self.signs_colors.get('data'))
+                stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
             else:
                 self._format(m, stream, indent, 1, context, level)
-                stream.write(self.signs_colors.get('comma') + ',\n' + self.signs_colors.get('data') + ' ' * indent)
+                stream.write(self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent)
 
     _dispatch[_collections.ChainMap.__repr__] = _pprint_chain_map
 
     def _pprint_deque(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.signs_colors.get('parenthesis') + '(' + self.signs_colors.get('data'))
+        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
         indent += len(cls.__name__) + 1
-        stream.write(self.signs_colors.get('square-brackets') + '[' + self.signs_colors.get('data'))
+        stream.write(self.sign_colors.get('square-brackets') + '[' + self.sign_colors.get('data'))
         if obj.maxlen is None:
             self._format_items(obj, stream, indent, allowance + 2,
                                context, level)
-            stream.write(self.signs_colors.get('square-brackets') + ']' + self.signs_colors.get('parenthesis') + ')' +
-                         self.signs_colors.get('data'))
+            stream.write(self.sign_colors.get('square-brackets') + ']' + self.sign_colors.get('parenthesis') + ')' +
+                         self.sign_colors.get('data'))
         else:
             self._format_items(obj, stream, indent, 2,
                                context, level)
             rml = self._repr(obj.maxlen, context, level)
-            stream.write(self.signs_colors.get('square-brackets') + ']' + self.signs_colors.get('comma') +
-                         ',' + self.signs_colors.get('data') + '\n' + (' ' * indent) + 'maxlen=' + rml +
-                         self.signs_colors.get('parenthesis') + ')')
+            stream.write(self.sign_colors.get('square-brackets') + ']' + self.sign_colors.get('comma') +
+                         ',' + self.sign_colors.get('data') + '\n' + (' ' * indent) + 'maxlen=' + rml +
+                         self.sign_colors.get('parenthesis') + ')')
 
     _dispatch[_collections.deque.__repr__] = _pprint_deque
 
     def _pprint_user_dict(self, obj, stream, indent, allowance, context, level):
         self._format(obj.data, stream, indent, allowance, context, level - 1)
 
     _dispatch[_collections.UserDict.__repr__] = _pprint_user_dict
@@ -561,9 +561,9 @@
 
     _dispatch[_collections.UserString.__repr__] = _pprint_user_string
 
 
 def pformat(obj, indent=1, width=80, depth=None, signs_colors: _Optional[_Mapping[str, str]] = None, *, compact=False,
             sort_dicts=True, underscore_numbers=False, **kwargs):
     """Format a Python object into a pretty-printed representation."""
-    return PrettyPrinter(indent=indent, width=width, depth=depth, compact=compact, signs_colors=signs_colors,
+    return PrettyPrinter(indent=indent, width=width, depth=depth, compact=compact, sign_colors=signs_colors,
                          sort_dicts=sort_dicts, underscore_numbers=underscore_numbers, **kwargs).pformat(obj)
```

### Comparing `log21-2.5.2/log21/ProgressBar.py` & `log21-2.5.3/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/StreamHandler.py` & `log21-2.5.3/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/log21/TreePrint.py` & `log21-2.5.3/log21/TreePrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 from typing import Union as _Union, Mapping as _Mapping, Sequence as _Sequence, Optional as _Optional, List as _List
 
 from log21.Colors import get_colors as _gc
 
 
 class TreePrint:
     class Node:
-        colors = {
-            'branches': _gc('Green'),
-            'fruit': _gc('LightMagenta'),
-        }
-
         def __init__(self, value: _Union[str, int], children: _Optional[_List[TreePrint.Node]] = None, indent: int = 4,
                      colors: _Optional[_Mapping[str, str]] = None, mode: str='-'):
             self.value = str(value)
             if children:
                 self._children = children
             else:
                 self._children = []
             self.indent = indent
-            self.colors = self.colors.copy()
+            self.colors = {
+                'branches': _gc('Green'),
+                'fruit': _gc('LightMagenta'),
+            }
+
             if colors:
                 for key, value in colors.items():
                     if key in self.colors:
                         self.colors[key] = _gc(value)
             if not mode:
                 self.mode = 1
             else:
```

### Comparing `log21-2.5.2/log21/__init__.py` & `log21-2.5.3/log21/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.5.2"
+__version__ = "2.5.3"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
```

### Comparing `log21-2.5.2/log21.egg-info/PKG-INFO` & `log21-2.5.3/log21.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.2
+Version: 2.5.3
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -71,17 +71,21 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.2
+### 2.5.3
 
-Improved type-hintings.
+Moved some dictionaries to `__init__` methods.
+`colors` in `Argparse.ColorizingHelpFormatter` class.
+`_level_name` in `Formatters._Formatter` class and `level_colors` in `Formatters.ColorizingFormatter` class.
+`sign_colors` in `PPrint.PrettyPrinter` class.
+`colors` in `TreePrint.TreePrint.Node` class.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.2/log21.egg-info/SOURCES.txt` & `log21-2.5.3/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.2/pyproject.toml` & `log21-2.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,13 +21,13 @@
   "Operating System :: Unix",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
   "webcolors"
 ]
-version = "2.5.2"
+version = "2.5.3"
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
 Source = "https://github.com/MPCodeWriter21/log21"
```

