# Comparing `tmp/findlike-0.1.tar.gz` & `tmp/findlike-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findlike-0.1.tar", last modified: Tue Jun 27 14:28:18 2023, max compression
+gzip compressed data, was "findlike-0.2.tar", last modified: Tue Jun 27 15:00:56 2023, max compression
```

## Comparing `findlike-0.1.tar` & `findlike-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-27 14:28:18.642032 findlike-0.1/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-0.1/LICENSE
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4443 2023-06-27 14:28:18.642032 findlike-0.1/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3840 2023-06-27 14:18:20.000000 findlike-0.1/README.md
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-27 14:28:18.638699 findlike-0.1/findlike/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-0.1/findlike/__init__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-0.1/findlike/__main__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5195 2023-06-27 02:31:26.000000 findlike-0.1/findlike/cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4226 2023-06-26 21:04:11.000000 findlike-0.1/findlike/format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3537 2023-06-26 19:22:52.000000 findlike-0.1/findlike/preprocessing.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2190 2023-06-23 20:43:15.000000 findlike-0.1/findlike/wrappers.py
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-27 14:28:18.642032 findlike-0.1/findlike.egg-info/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4443 2023-06-27 14:28:18.000000 findlike-0.1/findlike.egg-info/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      319 2023-06-27 14:28:18.000000 findlike-0.1/findlike.egg-info/SOURCES.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-06-27 14:28:18.000000 findlike-0.1/findlike.egg-info/dependency_links.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-06-27 14:28:18.000000 findlike-0.1/findlike.egg-info/entry_points.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-06-27 14:28:18.000000 findlike-0.1/findlike.egg-info/top_level.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      746 2023-06-27 14:26:37.000000 findlike-0.1/pyproject.toml
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-06-27 14:28:18.642032 findlike-0.1/setup.cfg
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-27 15:00:56.108324 findlike-0.2/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-0.2/LICENSE
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4443 2023-06-27 15:00:56.108324 findlike-0.2/PKG-INFO
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3840 2023-06-27 14:18:20.000000 findlike-0.2/README.md
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-27 15:00:56.108324 findlike-0.2/findlike/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-0.2/findlike/__init__.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-0.2/findlike/__main__.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5195 2023-06-27 02:31:26.000000 findlike-0.2/findlike/cli.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4226 2023-06-26 21:04:11.000000 findlike-0.2/findlike/format.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3537 2023-06-26 19:22:52.000000 findlike-0.2/findlike/preprocessing.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2190 2023-06-23 20:43:15.000000 findlike-0.2/findlike/wrappers.py
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-27 15:00:56.108324 findlike-0.2/findlike.egg-info/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4443 2023-06-27 15:00:56.000000 findlike-0.2/findlike.egg-info/PKG-INFO
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)      319 2023-06-27 15:00:56.000000 findlike-0.2/findlike.egg-info/SOURCES.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-06-27 15:00:56.000000 findlike-0.2/findlike.egg-info/dependency_links.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-06-27 15:00:56.000000 findlike-0.2/findlike.egg-info/entry_points.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-06-27 15:00:56.000000 findlike-0.2/findlike.egg-info/top_level.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)      746 2023-06-27 14:54:03.000000 findlike-0.2/pyproject.toml
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-06-27 15:00:56.108324 findlike-0.2/setup.cfg
```

### Comparing `findlike-0.1/LICENSE` & `findlike-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findlike-0.1/PKG-INFO` & `findlike-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlike
-Version: 0.1
+Version: 0.2
 Summary: findlike is a package to retrieve similar documents
 Author-email: Bruno Arine <bruno.arine@runbox.com>
 Project-URL: Homepage, http://www.github.com/brunoarine/findlike
 Project-URL: Repository, https://github.com/brunoarine/findlike.git
 Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `findlike-0.1/README.md` & `findlike-0.2/README.md`

 * *Files identical despite different names*

### Comparing `findlike-0.1/findlike/cli.py` & `findlike-0.2/findlike/cli.py`

 * *Files identical despite different names*

### Comparing `findlike-0.1/findlike/format.py` & `findlike-0.2/findlike/format.py`

 * *Files identical despite different names*

### Comparing `findlike-0.1/findlike/preprocessing.py` & `findlike-0.2/findlike/preprocessing.py`

 * *Files identical despite different names*

### Comparing `findlike-0.1/findlike/wrappers.py` & `findlike-0.2/findlike/wrappers.py`

 * *Files identical despite different names*

### Comparing `findlike-0.1/findlike.egg-info/PKG-INFO` & `findlike-0.2/findlike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlike
-Version: 0.1
+Version: 0.2
 Summary: findlike is a package to retrieve similar documents
 Author-email: Bruno Arine <bruno.arine@runbox.com>
 Project-URL: Homepage, http://www.github.com/brunoarine/findlike
 Project-URL: Repository, https://github.com/brunoarine/findlike.git
 Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `findlike-0.1/pyproject.toml` & `findlike-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "findlike"
-version = "0.1"
+version = "0.2"
 authors = [{ name = "Bruno Arine", email = "bruno.arine@runbox.com" }]
 description = "findlike is a package to retrieve similar documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

