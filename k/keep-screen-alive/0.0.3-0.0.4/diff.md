# Comparing `tmp/keep_screen_alive-0.0.3.tar.gz` & `tmp/keep_screen_alive-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keep_screen_alive-0.0.3.tar", max compression
+gzip compressed data, was "keep_screen_alive-0.0.4.tar", max compression
```

## Comparing `keep_screen_alive-0.0.3.tar` & `keep_screen_alive-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      420 2023-06-07 12:46:58.543143 keep_screen_alive-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-07 11:46:26.196161 keep_screen_alive-0.0.3/keep_alive/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-12 18:52:51.866839 keep_screen_alive-0.0.3/keep_alive/run.py
--rw-r--r--   0        0        0      778 2023-06-12 18:55:54.616161 keep_screen_alive-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 keep_screen_alive-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      477 2023-06-27 19:45:21.990191 keep_screen_alive-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 11:46:26.196161 keep_screen_alive-0.0.4/keep_alive/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-12 18:52:51.866839 keep_screen_alive-0.0.4/keep_alive/run.py
+-rw-r--r--   0        0        0      772 2023-06-27 19:47:46.877876 keep_screen_alive-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 keep_screen_alive-0.0.4/PKG-INFO
```

### Comparing `keep_screen_alive-0.0.3/keep_alive/run.py` & `keep_screen_alive-0.0.4/keep_alive/run.py`

 * *Files identical despite different names*

### Comparing `keep_screen_alive-0.0.3/pyproject.toml` & `keep_screen_alive-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "keep-screen-alive"
-version = "0.0.3"
-description = "A tool to keep your machine from going to sleep for some amount of time"
+version = "0.0.4"
+description = "A thin wrapper around macos caffeinate to use a relative datetime"
 authors = ["Tim Willis"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "keep_alive"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `keep_screen_alive-0.0.3/PKG-INFO` & `keep_screen_alive-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: keep-screen-alive
-Version: 0.0.3
-Summary: A tool to keep your machine from going to sleep for some amount of time
+Version: 0.0.4
+Summary: A thin wrapper around macos caffeinate to use a relative datetime
 License: MIT
 Author: Tim Willis
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## Summary
 A simple command line wrapper for [caffeinate](https://ss64.com/osx/caffeinate.html) on macOS that provides a forward looking relative datetime interface.
 
+## Install
+
+```bash
+$ pip install keep-screen-alive
+```
+
 ## Examples
 
 ```bash
 $ date
 Wed Jun  1 08:00:00 CDT 2023
 
 $ keep-alive 2h
```

