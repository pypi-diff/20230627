# Comparing `tmp/todo_by-1.1.0.tar.gz` & `tmp/todo_by-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todo_by-1.1.0.tar", last modified: Wed May 17 12:09:22 2023, max compression
+gzip compressed data, was "todo_by-1.2.0.tar", last modified: Tue Jun 27 11:49:29 2023, max compression
```

## Comparing `todo_by-1.1.0.tar` & `todo_by-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 12:09:22.399183 todo_by-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     2807 2023-05-17 12:09:22.397181 todo_by-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1572 2023-05-16 05:48:59.000000 todo_by-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 12:09:22.400181 todo_by-1.1.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      982 2023-05-17 12:09:08.000000 todo_by-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 12:09:22.313311 todo_by-1.1.0/todo_by/
--rwxr-xr-x   0 root         (0) root         (0)       50 2023-05-16 05:06:54.000000 todo_by-1.1.0/todo_by/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      646 2023-05-17 12:07:01.000000 todo_by-1.1.0/todo_by/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 12:09:22.379182 todo_by-1.1.0/todo_by.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2807 2023-05-17 12:09:22.000000 todo_by-1.1.0/todo_by.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-17 12:09:22.000000 todo_by-1.1.0/todo_by.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 12:09:22.000000 todo_by-1.1.0/todo_by.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-17 12:09:22.000000 todo_by-1.1.0/todo_by.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:49:29.719121 todo_by-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-27 11:49:29.719121 todo_by-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-27 11:49:20.000000 todo_by-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:49:29.719121 todo_by-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-06-27 11:49:20.000000 todo_by-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:49:29.715121 todo_by-1.2.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2659 2023-06-27 11:49:20.000000 todo_by-1.2.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:49:29.719121 todo_by-1.2.0/todo_by/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-27 11:49:20.000000 todo_by-1.2.0/todo_by/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1320 2023-06-27 11:49:20.000000 todo_by-1.2.0/todo_by/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-06-27 11:49:20.000000 todo_by-1.2.0/todo_by/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:49:29.719121 todo_by-1.2.0/todo_by.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-27 11:49:29.000000 todo_by-1.2.0/todo_by.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-27 11:49:29.000000 todo_by-1.2.0/todo_by.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:49:29.000000 todo_by-1.2.0/todo_by.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 11:49:29.000000 todo_by-1.2.0/todo_by.egg-info/top_level.txt
```

### Comparing `todo_by-1.1.0/README.md` & `todo_by-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,36 +3,53 @@
 Runtime lifetimes for comments. Inspired by
 [parker-codes/todo_by](https://github.com/parker-codes/todo_by).
 
 To use the library, install it using `pip`:
 
 
 ```bash
-pip install todo_by
+$ pip install todo_by
+
 ```
 
-Then import and use it like so:
+Import and call the `todo_by` decorator and add a date like so:
 
 ```python
-from todo_by import todo_by
+from todo_by import todo_by, todo_while
 
-@todo_by("2023-06-01")
+@todo_by("2050-06-01")
 def my_function():
-    # TODO: Implement this function by June 1st, 2023
+    # TODO: Implement this function by June 1st, 2050
 ```
-If the current date is after June 1st, 2023, the `todo_by` decorator will
-generate a `RuntimeError` with the message `"TODO by Jun 1, 2023 has passed"`.  
-If the current date is on or before June 1st, 2023, the code will run normally.
+
+If the current date is after June 1st, 2050, the `todo_by` decorator will
+generate a `RuntimeError` with the message `"TODO by Jun 1, 2050 has passed"`.  
+If the current date is on or before June 1st, 2030, the code will run normally.
 
 You can also add specific TODO comments:
 
 ```python
-@todo_by("2023-06-01", "Clean up implementation")
+@todo_by("2050-06-01", "Clean up implementation")
+```
+
+The `todo_while` decorator allows you to ensure todos are done based on a [SemVer
+requirement](https://semver.org/). This also allows you to make blockers:
+
+```python
+@todo_while("1.0.0", "setup.py", "This has to be in the first major release")
+def my_function():
+   self.assertTrue(True)
 ```
 
+If the current version in your `setup.py` (specify any file used for versioning
+your code) is equal or greater than 1.0.0, the `todo_while` decorator will
+generate a `RuntimeError` with the message 
+`"TODO version requirement '1.0.0' not satisfied by current <version_number>"`.  
+If the current version number is smaller than 1.0.0, the code will run normally.
+
 ## License:
 
 ```
 Copyright 2023 Martin Simon
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `todo_by-1.1.0/setup.py` & `todo_by-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='todo_by',
-    version='1.1.0',
+    version='1.2.0',
     author='Martin Simon',
     author_email='me@martinsimon.me',
     description=' Runtime lifetimes for comments.',
     url='https://github.com/barnumbirr/todo_by',
     download_url='https://github.com/barnumbirr/todo_by/archive/refs/heads/master.zip',
     packages=['todo_by'],
     long_description=long_description,
```

