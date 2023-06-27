# Comparing `tmp/consolecmdtools-4.0.0.tar.gz` & `tmp/consolecmdtools-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolecmdtools-4.0.0.tar", last modified: Tue Jun 27 07:13:57 2023, max compression
+gzip compressed data, was "consolecmdtools-4.0.1.tar", last modified: Tue Jun 27 07:17:36 2023, max compression
```

## Comparing `consolecmdtools-4.0.0.tar` & `consolecmdtools-4.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:57.386891 consolecmdtools-4.0.0/
--rw-rw-rw-   0        0        0     1082 2022-12-15 10:24:01.000000 consolecmdtools-4.0.0/LICENSE
--rw-rw-rw-   0        0        0     7808 2023-06-27 07:13:57.386891 consolecmdtools-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-06-27 07:10:47.000000 consolecmdtools-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:57.353803 consolecmdtools-4.0.0/consolecmdtools/
--rw-rw-rw-   0        0        0    16844 2023-06-27 07:12:50.000000 consolecmdtools-4.0.0/consolecmdtools/__init__.py
--rw-rw-rw-   0        0        0     2088 2022-12-15 11:28:48.000000 consolecmdtools-4.0.0/consolecmdtools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:57.382374 consolecmdtools-4.0.0/consolecmdtools.egg-info/
--rw-rw-rw-   0        0        0     7808 2023-06-27 07:13:57.000000 consolecmdtools-4.0.0/consolecmdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-27 07:13:57.000000 consolecmdtools-4.0.0/consolecmdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:13:57.000000 consolecmdtools-4.0.0/consolecmdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-27 07:13:57.000000 consolecmdtools-4.0.0/consolecmdtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 07:13:57.000000 consolecmdtools-4.0.0/consolecmdtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1265 2023-06-21 05:25:28.000000 consolecmdtools-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 07:13:57.387889 consolecmdtools-4.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:57.385891 consolecmdtools-4.0.0/tests/
--rw-rw-rw-   0        0        0    12980 2023-06-27 06:46:29.000000 consolecmdtools-4.0.0/tests/test_consolecmdtools.py
--rw-rw-rw-   0        0        0      363 2021-01-03 08:07:34.000000 consolecmdtools-4.0.0/tests/test_runas.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:17:36.728590 consolecmdtools-4.0.1/
+-rw-rw-rw-   0        0        0     1082 2022-12-15 10:24:01.000000 consolecmdtools-4.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7826 2023-06-27 07:17:36.728590 consolecmdtools-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5708 2023-06-27 07:16:35.000000 consolecmdtools-4.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:17:36.700027 consolecmdtools-4.0.1/consolecmdtools/
+-rw-rw-rw-   0        0        0    16853 2023-06-27 07:16:55.000000 consolecmdtools-4.0.1/consolecmdtools/__init__.py
+-rw-rw-rw-   0        0        0     2088 2022-12-15 11:28:48.000000 consolecmdtools-4.0.1/consolecmdtools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:17:36.724587 consolecmdtools-4.0.1/consolecmdtools.egg-info/
+-rw-rw-rw-   0        0        0     7826 2023-06-27 07:17:36.000000 consolecmdtools-4.0.1/consolecmdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-27 07:17:36.000000 consolecmdtools-4.0.1/consolecmdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:17:36.000000 consolecmdtools-4.0.1/consolecmdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-27 07:17:36.000000 consolecmdtools-4.0.1/consolecmdtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 07:17:36.000000 consolecmdtools-4.0.1/consolecmdtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1265 2023-06-21 05:25:28.000000 consolecmdtools-4.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:17:36.729586 consolecmdtools-4.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 07:17:36.727584 consolecmdtools-4.0.1/tests/
+-rw-rw-rw-   0        0        0    12980 2023-06-27 06:46:29.000000 consolecmdtools-4.0.1/tests/test_consolecmdtools.py
+-rw-rw-rw-   0        0        0      363 2021-01-03 08:07:34.000000 consolecmdtools-4.0.1/tests/test_runas.py
```

### Comparing `consolecmdtools-4.0.0/LICENSE` & `consolecmdtools-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consolecmdtools-4.0.0/PKG-INFO` & `consolecmdtools-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolecmdtools
-Version: 4.0.0
+Version: 4.0.1
 Summary: Console command tools in Python
 Author-email: Kyan <kai@kyan001.com>
 License: MIT License
         
         Copyright (c) 2020 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -143,17 +143,17 @@
 
 >>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
 ['/path/to/file1', '/path/to/file2']
 
 >>> cct.select_path(dir=True)  # Show file dialog to get dir path.
 '/path/to/dir'
 
->>> cct.show_in_dir("/path/to/file")  # Show file in Explorer/Finder/File Manager.
+>>> cct.show_in_file_manager("/path/to/file")  # Show file in Explorer/Finder/File Manager.
 
->>> cct.show_in_dir("/path/to/file", ask=True)  # Ask before show.
+>>> cct.show_in_file_manager("/path/to/file", ask=True)  # Ask before show.
 
 >>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
 [  # you can use `"\n".join(diff)` to print the diff.
     "-str1",
     "+str2"
 ]
```

### Comparing `consolecmdtools-4.0.0/README.md` & `consolecmdtools-4.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 
 >>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
 ['/path/to/file1', '/path/to/file2']
 
 >>> cct.select_path(dir=True)  # Show file dialog to get dir path.
 '/path/to/dir'
 
->>> cct.show_in_dir("/path/to/file")  # Show file in Explorer/Finder/File Manager.
+>>> cct.show_in_file_manager("/path/to/file")  # Show file in Explorer/Finder/File Manager.
 
->>> cct.show_in_dir("/path/to/file", ask=True)  # Ask before show.
+>>> cct.show_in_file_manager("/path/to/file", ask=True)  # Ask before show.
 
 >>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
 [  # you can use `"\n".join(diff)` to print the diff.
     "-str1",
     "+str2"
 ]
```

### Comparing `consolecmdtools-4.0.0/consolecmdtools/__init__.py` & `consolecmdtools-4.0.1/consolecmdtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import urllib.request
 import json
 import io
 # !! some imports are lazy-loaded
 
 import consoleiotools as cit
 
-__version__ = '4.0.0'
+__version__ = '4.0.1'
 
 
 def banner(text: str) -> str:
     """Generate a banner of 3 lines"""
     FILLER = "#"
     text = text.strip()
     middle_line = FILLER + text.center(int(len(text) / 0.618)) + FILLER
@@ -242,15 +242,15 @@
         path = tkinter.filedialog.askopenfilenames(*args, **kwargs)
     else:
         path = tkinter.filedialog.askopenfilename(*args, **kwargs)
     tkapp.destroy()
     return path
 
 
-def show_in_dir(path: str, ask: bool = False):
+def show_in_file_manager(path: str, ask: bool = False):
     """Show file in Explorer/Finder/File Manager."""
     import subprocess
     import platform
     if ask:
         if sys.platform.startswith("win"):
             file_manager = "Explorer"
         elif platform.system() == "Darwin":
```

### Comparing `consolecmdtools-4.0.0/consolecmdtools/__main__.py` & `consolecmdtools-4.0.1/consolecmdtools/__main__.py`

 * *Files identical despite different names*

### Comparing `consolecmdtools-4.0.0/consolecmdtools.egg-info/PKG-INFO` & `consolecmdtools-4.0.1/consolecmdtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolecmdtools
-Version: 4.0.0
+Version: 4.0.1
 Summary: Console command tools in Python
 Author-email: Kyan <kai@kyan001.com>
 License: MIT License
         
         Copyright (c) 2020 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -143,17 +143,17 @@
 
 >>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
 ['/path/to/file1', '/path/to/file2']
 
 >>> cct.select_path(dir=True)  # Show file dialog to get dir path.
 '/path/to/dir'
 
->>> cct.show_in_dir("/path/to/file")  # Show file in Explorer/Finder/File Manager.
+>>> cct.show_in_file_manager("/path/to/file")  # Show file in Explorer/Finder/File Manager.
 
->>> cct.show_in_dir("/path/to/file", ask=True)  # Ask before show.
+>>> cct.show_in_file_manager("/path/to/file", ask=True)  # Ask before show.
 
 >>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
 [  # you can use `"\n".join(diff)` to print the diff.
     "-str1",
     "+str2"
 ]
```

### Comparing `consolecmdtools-4.0.0/pyproject.toml` & `consolecmdtools-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `consolecmdtools-4.0.0/tests/test_consolecmdtools.py` & `consolecmdtools-4.0.1/tests/test_consolecmdtools.py`

 * *Files identical despite different names*

