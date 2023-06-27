# Comparing `tmp/orbit_component_dbshell-0.0.92.tar.gz` & `tmp/orbit_component_dbshell-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_dbshell-0.0.92.tar", max compression
+gzip compressed data, was "orbit_component_dbshell-1.0.2.tar", max compression
```

## Comparing `orbit_component_dbshell-0.0.92.tar` & `orbit_component_dbshell-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-17 16:50:03.098236 orbit_component_dbshell-0.0.92/LICENSE.md
--rw-r--r--   0        0        0        0 2023-06-21 15:30:58.376561 orbit_component_dbshell-0.0.92/README.md
--rw-r--r--   0        0        0       82 2023-06-21 12:41:11.901965 orbit_component_dbshell-0.0.92/orbit_component_dbshell/__init__.py
--rw-r--r--   0        0        0     1141 2023-06-23 14:41:23.687032 orbit_component_dbshell-0.0.92/orbit_component_dbshell/plugin.py
--rw-r--r--   0        0        0     1254 2023-06-27 14:46:36.450230 orbit_component_dbshell-0.0.92/pyproject.toml
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 orbit_component_dbshell-0.0.92/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 16:50:03.098236 orbit_component_dbshell-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-06-21 15:30:58.376561 orbit_component_dbshell-1.0.2/README.md
+-rw-r--r--   0        0        0       82 2023-06-21 12:41:11.901965 orbit_component_dbshell-1.0.2/orbit_component_dbshell/__init__.py
+-rw-r--r--   0        0        0     1141 2023-06-23 14:41:23.687032 orbit_component_dbshell-1.0.2/orbit_component_dbshell/plugin.py
+-rw-r--r--   0        0        0     1253 2023-06-27 14:51:54.407550 orbit_component_dbshell-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 orbit_component_dbshell-1.0.2/PKG-INFO
```

### Comparing `orbit_component_dbshell-0.0.92/orbit_component_dbshell/plugin.py` & `orbit_component_dbshell-1.0.2/orbit_component_dbshell/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_dbshell-0.0.92/pyproject.toml` & `orbit_component_dbshell-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-dbshell"
-version = "0.0.92"
+version = "1.0.2"
 description = "Orbit Database shell component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_dbshell"}]
 classifiers = [
```

### Comparing `orbit_component_dbshell-0.0.92/PKG-INFO` & `orbit_component_dbshell-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-dbshell
-Version: 0.0.92
+Version: 1.0.2
 Summary: Orbit Database shell component
 Home-page: https://gitlab.com/madpenguin/orbit-component-dbshell
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

