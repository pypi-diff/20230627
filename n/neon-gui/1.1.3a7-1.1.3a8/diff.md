# Comparing `tmp/neon_gui-1.1.3a7.tar.gz` & `tmp/neon_gui-1.1.3a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_gui-1.1.3a7.tar", last modified: Fri Jun 23 22:18:55 2023, max compression
+gzip compressed data, was "neon_gui-1.1.3a8.tar", last modified: Tue Jun 27 21:41:13 2023, max compression
```

## Comparing `neon_gui-1.1.3a7.tar` & `neon_gui-1.1.3a8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:18:55.529433 neon_gui-1.1.3a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-23 22:18:55.529433 neon_gui-1.1.3a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:18:55.529433 neon_gui-1.1.3a7/neon_gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/neon_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/neon_gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/neon_gui/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/neon_gui/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/neon_gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:18:55.529433 neon_gui-1.1.3a7/neon_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-23 22:18:55.000000 neon_gui-1.1.3a7/neon_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 22:18:55.000000 neon_gui-1.1.3a7/neon_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:18:55.000000 neon_gui-1.1.3a7/neon_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 22:18:55.000000 neon_gui-1.1.3a7/neon_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-23 22:18:55.000000 neon_gui-1.1.3a7/neon_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 22:18:55.000000 neon_gui-1.1.3a7/neon_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:18:55.529433 neon_gui-1.1.3a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-23 22:18:50.000000 neon_gui-1.1.3a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/neon_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/neon_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/setup.py
```

### Comparing `neon_gui-1.1.3a7/LICENSE.md` & `neon_gui-1.1.3a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/PKG-INFO` & `neon_gui-1.1.3a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_gui
-Version: 1.1.3a7
+Version: 1.1.3a8
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.1.3a7/README.md` & `neon_gui-1.1.3a8/README.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/neon_gui/__init__.py` & `neon_gui-1.1.3a8/neon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/neon_gui/__main__.py` & `neon_gui-1.1.3a8/neon_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/neon_gui/cli.py` & `neon_gui-1.1.3a8/neon_gui/cli.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/neon_gui/service.py` & `neon_gui-1.1.3a8/neon_gui/service.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/neon_gui/utils.py` & `neon_gui-1.1.3a8/neon_gui/utils.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a7/neon_gui.egg-info/PKG-INFO` & `neon_gui-1.1.3a8/neon_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.1.3a7
+Version: 1.1.3a8
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.1.3a7/setup.py` & `neon_gui-1.1.3a8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,12 +74,13 @@
     author='Neongecko',
     author_email='developers@neon.ai',
     description="Neon GUI Module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
+            # TODO: Deprecate `neon_gui_service` entrypoint
             'neon_gui_service=neon_gui.__main__:main',
             'neon-gui=neon_gui.cli:neon_gui_cli'
         ]
     }
 )
```

