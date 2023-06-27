# Comparing `tmp/strace-process-tree-1.3.0.tar.gz` & `tmp/strace-process-tree-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strace-process-tree-1.3.0.tar", last modified: Wed May 24 07:38:20 2023, max compression
+gzip compressed data, was "strace-process-tree-1.4.0.tar", last modified: Tue Jun 27 06:44:35 2023, max compression
```

## Comparing `strace-process-tree-1.3.0.tar` & `strace-process-tree-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/
--rw-r--r--   0 mg        (1000) mg        (1000)      126 2019-08-22 13:46:49.000000 strace-process-tree-1.3.0/.coveragerc
--rw-r--r--   0 mg        (1000) mg        (1000)       71 2019-08-21 13:01:00.000000 strace-process-tree-1.3.0/.gitignore
--rw-rw-r--   0 mg        (1000) mg        (1000)     3354 2023-05-24 07:37:21.000000 strace-process-tree-1.3.0/CHANGES.rst
--rw-r--r--   0 mg        (1000) mg        (1000)    18092 2019-08-21 13:59:11.000000 strace-process-tree-1.3.0/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      175 2019-08-21 14:00:54.000000 strace-process-tree-1.3.0/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)      366 2020-10-24 10:07:13.000000 strace-process-tree-1.3.0/Makefile
--rw-rw-r--   0 mg        (1000) mg        (1000)     3611 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)     2404 2020-11-30 19:57:48.000000 strace-process-tree-1.3.0/README.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      870 2022-10-28 06:33:45.000000 strace-process-tree-1.3.0/appveyor.yml
--rw-r--r--   0 mg        (1000) mg        (1000)       44 2019-08-21 13:47:16.000000 strace-process-tree-1.3.0/pytest.ini
--rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 strace-process-tree-1.3.0/release.mk
--rw-r--r--   0 mg        (1000) mg        (1000)      397 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/setup.cfg
--rwxrwxr-x   0 mg        (1000) mg        (1000)     1984 2022-10-28 06:37:52.000000 strace-process-tree-1.3.0/setup.py
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/strace_process_tree.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     3611 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      514 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/entry_points.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-08-21 12:43:27.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/not-zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)       20 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/top_level.txt
--rwxrwxr-x   0 mg        (1000) mg        (1000)    15300 2023-05-24 07:37:21.000000 strace-process-tree-1.3.0/strace_process_tree.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1126 2019-08-21 11:55:33.000000 strace-process-tree-1.3.0/strace_process_tree_example_output.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     7072 2019-08-21 11:55:33.000000 strace-process-tree-1.3.0/strace_process_tree_example_verbose_output.txt
--rw-r--r--   0 mg        (1000) mg        (1000)    19802 2023-05-24 07:32:02.000000 strace-process-tree-1.3.0/tests.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      710 2022-10-28 06:33:45.000000 strace-process-tree-1.3.0/tox.ini
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/
+-rw-r--r--   0 mg        (1000) mg        (1000)      126 2019-08-22 13:46:49.000000 strace-process-tree-1.4.0/.coveragerc
+-rw-r--r--   0 mg        (1000) mg        (1000)       71 2019-08-21 13:01:00.000000 strace-process-tree-1.4.0/.gitignore
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3527 2023-06-27 06:43:42.000000 strace-process-tree-1.4.0/CHANGES.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)    18092 2019-08-21 13:59:11.000000 strace-process-tree-1.4.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      175 2019-08-21 14:00:54.000000 strace-process-tree-1.4.0/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)      366 2020-10-24 10:07:13.000000 strace-process-tree-1.4.0/Makefile
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3498 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2404 2020-11-30 19:57:48.000000 strace-process-tree-1.4.0/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      841 2023-05-29 09:02:57.000000 strace-process-tree-1.4.0/appveyor.yml
+-rw-r--r--   0 mg        (1000) mg        (1000)       44 2019-08-21 13:47:16.000000 strace-process-tree-1.4.0/pytest.ini
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 strace-process-tree-1.4.0/release.mk
+-rw-rw-r--   0 mg        (1000) mg        (1000)      398 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/setup.cfg
+-rwxrwxr-x   0 mg        (1000) mg        (1000)     1872 2023-05-30 10:47:10.000000 strace-process-tree-1.4.0/setup.py
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/strace_process_tree.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     3498 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      514 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/entry_points.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-08-21 12:43:27.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/not-zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)       20 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/top_level.txt
+-rwxrwxr-x   0 mg        (1000) mg        (1000)    15372 2023-06-27 06:43:51.000000 strace-process-tree-1.4.0/strace_process_tree.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1126 2019-08-21 11:55:33.000000 strace-process-tree-1.4.0/strace_process_tree_example_output.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     7072 2019-08-21 11:55:33.000000 strace-process-tree-1.4.0/strace_process_tree_example_verbose_output.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)    19942 2023-06-27 06:40:05.000000 strace-process-tree-1.4.0/tests.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      700 2023-05-29 09:02:57.000000 strace-process-tree-1.4.0/tox.ini
```

### Comparing `strace-process-tree-1.3.0/CHANGES.rst` & `strace-process-tree-1.4.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changes
 =======
 
 
+1.4.0 (2023-06-27)
+------------------
+
+* Fix parsing `/* 1 var */` (`issue 9
+  <https://github.com/mgedmin/strace-process-tree/pull/9>`_).
+* Removed support for Python 2.
+
+
 1.3.0 (2023-05-24)
 ------------------
 
 * Support the NO_COLOR environment variable for disabling color autodetection
   (see https://no-color.org/).
 * Fix parsing '<... syscall resumed>)' lines without a space in front of
   the closing parenthesis (`issue 5
```

### Comparing `strace-process-tree-1.3.0/LICENSE` & `strace-process-tree-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.3.0/PKG-INFO` & `strace-process-tree-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: strace-process-tree
-Version: 1.3.0
+Version: 1.4.0
 Summary: Produce a process tree from an strace log
 Home-page: https://github.com/mgedmin/strace-process-tree
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL v2 or v3
 Keywords: strace log process tree
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 strace-process-tree
 ===================
 
 .. image:: https://github.com/mgedmin/strace-process-tree/workflows/build/badge.svg?branch=master
```

### Comparing `strace-process-tree-1.3.0/README.rst` & `strace-process-tree-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.3.0/appveyor.yml` & `strace-process-tree-1.4.0/appveyor.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 version: build-{build}-{branch}
 
 environment:
   matrix:
     # https://www.appveyor.com/docs/installed-software#python lists available
     # versions
-    - PYTHON: "C:\\Python27"
     - PYTHON: "C:\\Python37"
     - PYTHON: "C:\\Python38"
     - PYTHON: "C:\\Python39"
     - PYTHON: "C:\\Python310"
     - PYTHON: "C:\\Python311"
 
 init:
```

### Comparing `strace-process-tree-1.3.0/release.mk` & `strace-process-tree-1.4.0/release.mk`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.3.0/setup.py` & `strace-process-tree-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,25 +32,24 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     license="GPL v2 or v3",
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*",
+    python_requires=">=3.7",
 
     py_modules=["strace_process_tree"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "strace-process-tree = strace_process_tree:main",
         ],
```

### Comparing `strace-process-tree-1.3.0/strace_process_tree.egg-info/PKG-INFO` & `strace-process-tree-1.4.0/strace_process_tree.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: strace-process-tree
-Version: 1.3.0
+Version: 1.4.0
 Summary: Produce a process tree from an strace log
 Home-page: https://github.com/mgedmin/strace-process-tree
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL v2 or v3
 Keywords: strace log process tree
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 strace-process-tree
 ===================
 
 .. image:: https://github.com/mgedmin/strace-process-tree/workflows/build/badge.svg?branch=master
```

### Comparing `strace-process-tree-1.3.0/strace_process_tree.egg-info/SOURCES.txt` & `strace-process-tree-1.4.0/strace_process_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.3.0/strace_process_tree.py` & `strace-process-tree-1.4.0/strace_process_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re
 import string
 import sys
 from collections import defaultdict, namedtuple
 from functools import partial
 
 
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 __author__ = 'Marius Gedminas <marius@gedmin.as>'
 __url__ = "https://github.com/mgedmin/strace-process-tree"
 __licence__ = 'GPL v2 or v3'  # or ask me for MIT
 
 
 Tree = namedtuple('Tree', 'trunk, fork, end, space')
 
@@ -320,25 +320,26 @@
     if event.startswith('clone('):
         event = re.sub('[(].*, flags=([^,]*), .*[)]', r'(\1)', event)
     return event.rstrip()
 
 
 def extract_command_line(event):
     # execve("/usr/bin/foo", ["foo", "bar"], [/* 45 vars */]) => foo bar
+    # execve("/usr/bin/foo", ["foo", "bar"], [/* 1 var */]) => foo bar
     if event.startswith('clone('):
         if 'CLONE_THREAD' in event:
             return '(thread)'
         elif 'flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD' in event:
             return '(fork)'
         else:
             return '...'
     elif event.startswith('execve('):
         command = event.strip()
         command = re.sub(r'^execve\([^[]*\[', '', command)
-        command = re.sub(r'\], (0x[0-9a-f]+ )?\[?/\* \d+ vars \*/\]?\)$', '',
+        command = re.sub(r'\], (0x[0-9a-f]+ )?\[?/\* \d+ vars? \*/\]?\)$', '',
                          command)
         command = parse_argv(command)
         return format_command(command)
     else:
         return event.rstrip()
```

### Comparing `strace-process-tree-1.3.0/strace_process_tree_example_output.txt` & `strace-process-tree-1.4.0/strace_process_tree_example_output.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.3.0/strace_process_tree_example_verbose_output.txt` & `strace-process-tree-1.4.0/strace_process_tree_example_verbose_output.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.3.0/tests.py` & `strace-process-tree-1.4.0/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,19 @@
     )
     assert stp.extract_command_line(
         'execve("/usr/bin/foo", ["foo", "bar"], [/* 45 vars */])'
     ) == (
         'foo bar'
     )
     assert stp.extract_command_line(
+        'execve("/usr/bin/foo", ["short", "env"], [/* 1 var */])'
+    ) == (
+        'short env'
+    )
+    assert stp.extract_command_line(
         'clone(child_stack=NULL, flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD, child_tidptr=0x7fbb38e89a10)'
     ) == (
         '(fork)'
     )
     assert stp.extract_command_line(
         'clone(child_stack=0x7fbb3690dfb0, flags=CLONE_VM|CLONE_FS|CLONE_FILES|CLONE_SIGHAND|CLONE_THREAD|CLONE_SYSVSEM|CLONE_SETTLS|CLONE_PARENT_SETTID|CLONE_CHILD_CLEARTID, parent_tidptr=0x7fbb3690e9d0, tls=0x7fbb3690e700, child_tidptr=0x7fbb3690e9d0)'
     ) == (
```

### Comparing `strace-process-tree-1.3.0/tox.ini` & `strace-process-tree-1.4.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py27,py37,py38,py39,py310,py311,pypy,pypy3
+envlist = py37,py38,py39,py310,py311,pypy3
 
 [testenv]
 deps =
     pytest
 commands =
     pytest {posargs}
```

