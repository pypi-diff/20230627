# Comparing `tmp/contextplot-0.0.2.tar.gz` & `tmp/contextplot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextplot-0.0.2.tar", last modified: Mon Jun 26 23:44:30 2023, max compression
+gzip compressed data, was "contextplot-0.0.3.tar", last modified: Mon Jun 26 23:55:35 2023, max compression
```

## Comparing `contextplot-0.0.2.tar` & `contextplot-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:44:30.482838 contextplot-0.0.2/
--rw-r--r--   0 josh       (502) staff       (20)     1071 2023-06-26 23:19:09.000000 contextplot-0.0.2/LICENSE
--rw-r--r--   0 josh       (502) staff       (20)      811 2023-06-26 23:44:30.482726 contextplot-0.0.2/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      280 2023-06-26 20:39:14.000000 contextplot-0.0.2/README.md
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:44:30.481997 contextplot-0.0.2/contextplot/
--rw-r--r--   0 josh       (502) staff       (20)     6834 2023-06-26 23:40:29.000000 contextplot-0.0.2/contextplot/__init__.py
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:44:30.482568 contextplot-0.0.2/contextplot.egg-info/
--rw-r--r--   0 josh       (502) staff       (20)      811 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      239 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (502) staff       (20)        1 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (502) staff       (20)       25 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/requires.txt
--rw-r--r--   0 josh       (502) staff       (20)       12 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/top_level.txt
--rw-r--r--   0 josh       (502) staff       (20)      598 2023-06-26 23:43:12.000000 contextplot-0.0.2/pyproject.toml
--rw-r--r--   0 josh       (502) staff       (20)       38 2023-06-26 23:44:30.482875 contextplot-0.0.2/setup.cfg
--rw-r--r--   0 josh       (502) staff       (20)      339 2023-06-26 23:43:17.000000 contextplot-0.0.2/setup.py
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:55:35.675372 contextplot-0.0.3/
+-rw-r--r--   0 josh       (502) staff       (20)     1071 2023-06-26 23:19:09.000000 contextplot-0.0.3/LICENSE
+-rw-r--r--   0 josh       (502) staff       (20)      697 2023-06-26 23:55:35.675249 contextplot-0.0.3/PKG-INFO
+-rw-r--r--   0 josh       (502) staff       (20)      166 2023-06-26 23:54:31.000000 contextplot-0.0.3/README.md
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:55:35.674516 contextplot-0.0.3/contextplot/
+-rw-r--r--   0 josh       (502) staff       (20)     6834 2023-06-26 23:40:29.000000 contextplot-0.0.3/contextplot/__init__.py
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:55:35.675078 contextplot-0.0.3/contextplot.egg-info/
+-rw-r--r--   0 josh       (502) staff       (20)      697 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (502) staff       (20)      239 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (502) staff       (20)        1 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (502) staff       (20)       25 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/requires.txt
+-rw-r--r--   0 josh       (502) staff       (20)       12 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/top_level.txt
+-rw-r--r--   0 josh       (502) staff       (20)      598 2023-06-26 23:54:46.000000 contextplot-0.0.3/pyproject.toml
+-rw-r--r--   0 josh       (502) staff       (20)       38 2023-06-26 23:55:35.675410 contextplot-0.0.3/setup.cfg
+-rw-r--r--   0 josh       (502) staff       (20)      339 2023-06-26 23:54:46.000000 contextplot-0.0.3/setup.py
```

### Comparing `contextplot-0.0.2/LICENSE` & `contextplot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `contextplot-0.0.2/contextplot/__init__.py` & `contextplot-0.0.3/contextplot/__init__.py`

 * *Files identical despite different names*

### Comparing `contextplot-0.0.2/pyproject.toml` & `contextplot-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "Make Matplotlib plots in Jupyter notebooks using a context manager API"
 name = "contextplot"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.2"
+version = "0.0.3"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/joshburkart/joshpyutil/-/issues"
 "Homepage" = "https://gitlab.com/joshburkart/joshpyutil"
 
 [build-system]
 build-backend = "setuptools.build_meta"
```

