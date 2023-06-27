# Comparing `tmp/json-grep-1.2.0.tar.gz` & `tmp/json-grep-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-grep-1.2.0.tar", last modified: Mon May 15 09:15:30 2023, max compression
+gzip compressed data, was "json-grep-1.2.1.tar", last modified: Tue Jun 27 07:20:26 2023, max compression
```

## Comparing `json-grep-1.2.0.tar` & `json-grep-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.2.0/MANIFEST.in
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1654 2023-05-15 09:15:30.804437 json-grep-1.2.0/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1233 2023-05-15 09:06:17.000000 json-grep-1.2.0/README.md
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/json_grep.egg-info/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1654 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      368 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/SOURCES.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/dependency_links.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/entry_points.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-05-15 09:12:34.000000 json-grep-1.2.0/json_grep.egg-info/not-zip-safe
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/top_level.txt
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/jsongrep/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-05-15 09:05:59.000000 json-grep-1.2.0/jsongrep/VERSION
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.2.0/jsongrep/__init__.py
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/jsongrep/libs/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.2.0/jsongrep/libs/__init__.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     3343 2023-05-15 09:03:14.000000 json-grep-1.2.0/jsongrep/libs/json_filter.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.2.0/jsongrep/libs/setuptools.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     2347 2023-05-15 09:09:12.000000 json-grep-1.2.0/jsongrep/main.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-05-15 09:15:30.804437 json-grep-1.2.0/setup.cfg
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.2.0/setup.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.2.1/MANIFEST.in
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 07:20:26.620216 json-grep-1.2.1/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1372 2023-05-15 09:17:46.000000 json-grep-1.2.1/README.md
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/json_grep.egg-info/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/SOURCES.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/dependency_links.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/entry_points.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-05-15 09:12:34.000000 json-grep-1.2.1/json_grep.egg-info/not-zip-safe
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/top_level.txt
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/jsongrep/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-06-27 07:20:06.000000 json-grep-1.2.1/jsongrep/VERSION
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.2.1/jsongrep/__init__.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/jsongrep/libs/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.2.1/jsongrep/libs/__init__.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.2.1/jsongrep/libs/cli_colors.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     3420 2023-06-27 07:12:39.000000 json-grep-1.2.1/jsongrep/libs/json_filter.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.2.1/jsongrep/libs/setuptools.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2364 2023-06-27 07:00:36.000000 json-grep-1.2.1/jsongrep/main.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-06-27 07:20:26.620216 json-grep-1.2.1/setup.cfg
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.2.1/setup.py
```

### Comparing `json-grep-1.2.0/PKG-INFO` & `json-grep-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.2.0
+Version: 1.2.1
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,28 +16,31 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
-usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
+usage: json-grep [-h] [-m] [-v] [-e] filter_keys [filter_keys ...]
 
-JSON GREP is utility for filtering selected keys from json string piped from STDOUT
+JSON GREP v1.2.0 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
-  filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
-                        use '.' separator to specify how deep is key in dict tree structure.
+  filter_keys           List of keys which you want to filter from json dict.If key is in deeper level of tree 
+                        structure use '.' separator to specify how deep is key in dict tree structure.
+                        You can also use '*' at the end of key name to filter keys as 'beginning with'.
+                        You can also specify value of item which you want to pass only by operator '=' or
+                        '~'. '~' means that value is somewhere in string.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
-  -e, --show-errors     Ignore errors caused by json decode
+  -e, --show-errors     Show errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
```

### Comparing `json-grep-1.2.0/README.md` & `json-grep-1.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
-usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
+usage: json-grep [-h] [-m] [-v] [-e] filter_keys [filter_keys ...]
 
-JSON GREP is utility for filtering selected keys from json string piped from STDOUT
+JSON GREP v1.2.0 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
-  filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
-                        use '.' separator to specify how deep is key in dict tree structure.
+  filter_keys           List of keys which you want to filter from json dict.If key is in deeper level of tree 
+                        structure use '.' separator to specify how deep is key in dict tree structure.
+                        You can also use '*' at the end of key name to filter keys as 'beginning with'.
+                        You can also specify value of item which you want to pass only by operator '=' or
+                        '~'. '~' means that value is somewhere in string.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
-  -e, --show-errors     Ignore errors caused by json decode
+  -e, --show-errors     Show errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
```

### Comparing `json-grep-1.2.0/json_grep.egg-info/PKG-INFO` & `json-grep-1.2.1/json_grep.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.2.0
+Version: 1.2.1
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,28 +16,31 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
-usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
+usage: json-grep [-h] [-m] [-v] [-e] filter_keys [filter_keys ...]
 
-JSON GREP is utility for filtering selected keys from json string piped from STDOUT
+JSON GREP v1.2.0 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
-  filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
-                        use '.' separator to specify how deep is key in dict tree structure.
+  filter_keys           List of keys which you want to filter from json dict.If key is in deeper level of tree 
+                        structure use '.' separator to specify how deep is key in dict tree structure.
+                        You can also use '*' at the end of key name to filter keys as 'beginning with'.
+                        You can also specify value of item which you want to pass only by operator '=' or
+                        '~'. '~' means that value is somewhere in string.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
-  -e, --show-errors     Ignore errors caused by json decode
+  -e, --show-errors     Show errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
```

### Comparing `json-grep-1.2.0/jsongrep/libs/json_filter.py` & `json-grep-1.2.1/jsongrep/libs/json_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+from jsongrep.libs.cli_colors import CMD, FG
 
 
 class JsonFilterException(Exception):
     pass
 
 
 class JsonFilter:
@@ -74,11 +75,11 @@
 
     @staticmethod
     def format_result(data: dict, multiline_output: bool = False, values_only: bool = False) -> str:
         ret = ""
         for key, value in data.items():
             br_line = "\n" if multiline_output else " "
             if values_only:
-                ret = f"{ret}\33[33m{value}\33[0m{br_line}"
+                ret = f"{ret}{FG.cyan}{value}{CMD.reset}{br_line}"
             else:
-                ret = f"{ret}\"\33[32m{key}\33[0m\": \"\33[36m{value}\33[0m\"{br_line}"
+                ret = f"{ret}\"{FG.green}{CMD.bold}{key}{CMD.reset}\": \"{FG.cyan}{value}{CMD.reset}\"{br_line}"
         return f"{ret}\n"
```

### Comparing `json-grep-1.2.0/jsongrep/main.py` & `json-grep-1.2.1/jsongrep/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import signal
 import sys
 from argparse import ArgumentParser
-from .libs.setuptools import get_file_content
-from .libs.json_filter import JsonFilter, JsonFilterException
+from jsongrep.libs.setuptools import get_file_content
+from jsongrep.libs.json_filter import JsonFilter, JsonFilterException
 
 
 def _handle_exit(sig, frame):
     print('Terminated.')
     sys.exit(0)
 
 
 def _handle_args() -> tuple:
     version = get_file_content(os.path.join(os.path.dirname(__file__), "VERSION"))
     parser = ArgumentParser(description="JSON GREP v{version} is utility for filtering selected keys from json string piped from STDOUT".format(version=version))
     parser.add_argument("filter_keys", type=str, nargs="+", help=(
-        "List of keys which you want to filter from json dict."
+        "List of keys which you want to filter from json dict. "
         "If key is in deeper level of tree structure use '.' separator "
         "to specify how deep is key in dict tree structure. You can also use '*' "
         "at the end of key name to filter keys as 'beginning with'. "
         "You can also specify value of item which you want to pass "
         "only by operator '=' or '~'. '~' means "
         "that value is somewhere in string.")
                         )
```

### Comparing `json-grep-1.2.0/setup.py` & `json-grep-1.2.1/setup.py`

 * *Files identical despite different names*

