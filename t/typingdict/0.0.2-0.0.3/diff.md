# Comparing `tmp/typingdict-0.0.2.tar.gz` & `tmp/typingdict-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typingdict-0.0.2.tar", last modified: Tue Jun 27 11:47:53 2023, max compression
+gzip compressed data, was "typingdict-0.0.3.tar", last modified: Tue Jun 27 12:17:51 2023, max compression
```

## Comparing `typingdict-0.0.2.tar` & `typingdict-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:47:53.836656 typingdict-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 11:47:46.000000 typingdict-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-27 11:47:53.836656 typingdict-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-27 11:47:46.000000 typingdict-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:47:53.836656 typingdict-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 11:47:46.000000 typingdict-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:47:53.836656 typingdict-0.0.2/typingdict/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 11:47:46.000000 typingdict-0.0.2/typingdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 11:47:46.000000 typingdict-0.0.2/typingdict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 11:47:46.000000 typingdict-0.0.2/typingdict/beautifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-27 11:47:46.000000 typingdict-0.0.2/typingdict/typer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:47:53.836656 typingdict-0.0.2/typingdict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-27 11:47:53.000000 typingdict-0.0.2/typingdict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 11:47:53.000000 typingdict-0.0.2/typingdict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:47:53.000000 typingdict-0.0.2/typingdict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 11:47:53.000000 typingdict-0.0.2/typingdict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:17:51.424486 typingdict-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 12:17:38.000000 typingdict-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-27 12:17:51.424486 typingdict-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-27 12:17:38.000000 typingdict-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:17:51.424486 typingdict-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 12:17:38.000000 typingdict-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:17:51.424486 typingdict-0.0.3/typingdict/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 12:17:38.000000 typingdict-0.0.3/typingdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 12:17:38.000000 typingdict-0.0.3/typingdict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 12:17:38.000000 typingdict-0.0.3/typingdict/beautifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-27 12:17:38.000000 typingdict-0.0.3/typingdict/typer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:17:51.424486 typingdict-0.0.3/typingdict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-27 12:17:51.000000 typingdict-0.0.3/typingdict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 12:17:51.000000 typingdict-0.0.3/typingdict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:17:51.000000 typingdict-0.0.3/typingdict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 12:17:51.000000 typingdict-0.0.3/typingdict.egg-info/top_level.txt
```

### Comparing `typingdict-0.0.2/LICENSE` & `typingdict-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typingdict-0.0.2/PKG-INFO` & `typingdict-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typingdict
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate TypedDict Automatically
 Home-page: https://github.com/am230/typingdict
 Author: am230
 License: MIT Licence
 Keywords: Automation,Typing
 Platform: any
 Requires: strinpy
```

### Comparing `typingdict-0.0.2/setup.py` & `typingdict-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 author = 'am230'
 name = 'typingdict'
 py_modules = [name]
 
 setup(
     name=name,
-    version="0.0.2",
+    version='0.0.3',
     keywords=["Automation", "Typing"],
     description="Generate TypedDict Automatically",
     long_description=long_description,
     license="MIT Licence",
     long_description_content_type='text/x-rst',
     packages=find_packages(),
     requires=['strinpy', 'astor'],
```

### Comparing `typingdict-0.0.2/typingdict/typer.py` & `typingdict-0.0.3/typingdict/typer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Any
 import strinpy
 import keyword
 import re
 
 
 class Typer:
+    keywords = ['List', 'Dict', 'Union', 'TypedDict', 'Optional']
+    keywords.extend(keyword.kwlist)
+
     def __init__(self) -> None:
         self.parts: list[Any] = ['from typing import List, Dict, Union, TypedDict, Optional\n\n']
-        self.names: set[str] = set()
+        self.names: set[str] = set(self.keywords)
         self.dicts: dict[str, str] = {}
 
     def format_name(self, name: str) -> str:
         # convert snakecase to camelcase
         parts = name.split('_')
         name = ''.join([part.capitalize() for part in parts])
         if name not in self.names:
@@ -21,15 +24,15 @@
         while f'{name}{count}' in self.names:
             count += 1
         name = f'{name}{count}'
         self.names.add(name)
         return name
 
     def is_invalid_name(self, name: str) -> bool:
-        if keyword.iskeyword(name):
+        if keyword.iskeyword(name) or name in self.keywords:
             return True
         return not re.match(r'^[\w_][\w_\d]*$', name)
 
     def is_exists(self, name, attrs: dict) -> tuple[bool, str]:
         key = str(attrs)
         if key in self.dicts:
             return True, self.dicts[key]
```

### Comparing `typingdict-0.0.2/typingdict.egg-info/PKG-INFO` & `typingdict-0.0.3/typingdict.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typingdict
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate TypedDict Automatically
 Home-page: https://github.com/am230/typingdict
 Author: am230
 License: MIT Licence
 Keywords: Automation,Typing
 Platform: any
 Requires: strinpy
```

