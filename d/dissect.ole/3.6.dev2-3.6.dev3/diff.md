# Comparing `tmp/dissect.ole-3.6.dev2.tar.gz` & `tmp/dissect.ole-3.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ole-3.6.dev2.tar", last modified: Fri Jun 16 12:50:28 2023, max compression
+gzip compressed data, was "dissect.ole-3.6.dev3.tar", last modified: Tue Jun 27 07:49:13 2023, max compression
```

## Comparing `dissect.ole-3.6.dev2.tar` & `dissect.ole-3.6.dev3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:28.699264 dissect.ole-3.6.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-16 12:50:28.699264 dissect.ole-3.6.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:28.691264 dissect.ole-3.6.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:28.695264 dissect.ole-3.6.dev2/dissect/ole/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/dissect/ole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/dissect/ole/c_ole.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/dissect/ole/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/dissect/ole/ole.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:28.695264 dissect.ole-3.6.dev2/dissect.ole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-16 12:50:28.000000 dissect.ole-3.6.dev2/dissect.ole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 12:50:28.000000 dissect.ole-3.6.dev2/dissect.ole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:28.000000 dissect.ole-3.6.dev2/dissect.ole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:50:28.000000 dissect.ole-3.6.dev2/dissect.ole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:28.000000 dissect.ole-3.6.dev2/dissect.ole.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-16 12:50:17.000000 dissect.ole-3.6.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:28.699264 dissect.ole-3.6.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:28.691264 dissect.ole-3.6.dev2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:28.695264 dissect.ole-3.6.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-16 12:50:11.000000 dissect.ole-3.6.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:13.349745 dissect.ole-3.6.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-27 07:49:13.349745 dissect.ole-3.6.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:13.341746 dissect.ole-3.6.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:13.349745 dissect.ole-3.6.dev3/dissect/ole/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/dissect/ole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/dissect/ole/c_ole.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/dissect/ole/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/dissect/ole/ole.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:13.345745 dissect.ole-3.6.dev3/dissect.ole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-27 07:49:13.000000 dissect.ole-3.6.dev3/dissect.ole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 07:49:13.000000 dissect.ole-3.6.dev3/dissect.ole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:13.000000 dissect.ole-3.6.dev3/dissect.ole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:13.000000 dissect.ole-3.6.dev3/dissect.ole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:13.000000 dissect.ole-3.6.dev3/dissect.ole.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-27 07:49:03.000000 dissect.ole-3.6.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:13.349745 dissect.ole-3.6.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:13.341746 dissect.ole-3.6.dev3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:13.349745 dissect.ole-3.6.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-27 07:48:58.000000 dissect.ole-3.6.dev3/tox.ini
```

### Comparing `dissect.ole-3.6.dev2/LICENSE` & `dissect.ole-3.6.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/PKG-INFO` & `dissect.ole-3.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.6.dev2
+Version: 3.6.dev3
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ole-3.6.dev2/README.md` & `dissect.ole-3.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/dissect/ole/c_ole.py` & `dissect.ole-3.6.dev3/dissect/ole/c_ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/dissect/ole/ole.py` & `dissect.ole-3.6.dev3/dissect/ole/ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/dissect.ole.egg-info/PKG-INFO` & `dissect.ole-3.6.dev3/dissect.ole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.6.dev2
+Version: 3.6.dev3
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ole-3.6.dev2/pyproject.toml` & `dissect.ole-3.6.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/tests/docs/Makefile` & `dissect.ole-3.6.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/tests/docs/conf.py` & `dissect.ole-3.6.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.6.dev2/tox.ini` & `dissect.ole-3.6.dev3/tox.ini`

 * *Files identical despite different names*

