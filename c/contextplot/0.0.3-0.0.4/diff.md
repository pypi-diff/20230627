# Comparing `tmp/contextplot-0.0.3.tar.gz` & `tmp/contextplot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextplot-0.0.3.tar", last modified: Mon Jun 26 23:55:35 2023, max compression
+gzip compressed data, was "contextplot-0.0.4.tar", last modified: Tue Jun 27 00:03:56 2023, max compression
```

## Comparing `contextplot-0.0.3.tar` & `contextplot-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:55:35.675372 contextplot-0.0.3/
--rw-r--r--   0 josh       (502) staff       (20)     1071 2023-06-26 23:19:09.000000 contextplot-0.0.3/LICENSE
--rw-r--r--   0 josh       (502) staff       (20)      697 2023-06-26 23:55:35.675249 contextplot-0.0.3/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      166 2023-06-26 23:54:31.000000 contextplot-0.0.3/README.md
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:55:35.674516 contextplot-0.0.3/contextplot/
--rw-r--r--   0 josh       (502) staff       (20)     6834 2023-06-26 23:40:29.000000 contextplot-0.0.3/contextplot/__init__.py
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:55:35.675078 contextplot-0.0.3/contextplot.egg-info/
--rw-r--r--   0 josh       (502) staff       (20)      697 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      239 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (502) staff       (20)        1 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (502) staff       (20)       25 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/requires.txt
--rw-r--r--   0 josh       (502) staff       (20)       12 2023-06-26 23:55:35.000000 contextplot-0.0.3/contextplot.egg-info/top_level.txt
--rw-r--r--   0 josh       (502) staff       (20)      598 2023-06-26 23:54:46.000000 contextplot-0.0.3/pyproject.toml
--rw-r--r--   0 josh       (502) staff       (20)       38 2023-06-26 23:55:35.675410 contextplot-0.0.3/setup.cfg
--rw-r--r--   0 josh       (502) staff       (20)      339 2023-06-26 23:54:46.000000 contextplot-0.0.3/setup.py
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-27 00:03:56.299928 contextplot-0.0.4/
+-rw-r--r--   0 josh       (502) staff       (20)     1071 2023-06-26 23:19:09.000000 contextplot-0.0.4/LICENSE
+-rw-r--r--   0 josh       (502) staff       (20)      698 2023-06-27 00:03:56.299800 contextplot-0.0.4/PKG-INFO
+-rw-r--r--   0 josh       (502) staff       (20)      167 2023-06-27 00:03:19.000000 contextplot-0.0.4/README.md
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-27 00:03:56.299064 contextplot-0.0.4/contextplot/
+-rw-r--r--   0 josh       (502) staff       (20)     6834 2023-06-26 23:40:29.000000 contextplot-0.0.4/contextplot/__init__.py
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-27 00:03:56.299627 contextplot-0.0.4/contextplot.egg-info/
+-rw-r--r--   0 josh       (502) staff       (20)      698 2023-06-27 00:03:56.000000 contextplot-0.0.4/contextplot.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (502) staff       (20)      239 2023-06-27 00:03:56.000000 contextplot-0.0.4/contextplot.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (502) staff       (20)        1 2023-06-27 00:03:56.000000 contextplot-0.0.4/contextplot.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (502) staff       (20)       25 2023-06-27 00:03:56.000000 contextplot-0.0.4/contextplot.egg-info/requires.txt
+-rw-r--r--   0 josh       (502) staff       (20)       12 2023-06-27 00:03:56.000000 contextplot-0.0.4/contextplot.egg-info/top_level.txt
+-rw-r--r--   0 josh       (502) staff       (20)      598 2023-06-27 00:03:38.000000 contextplot-0.0.4/pyproject.toml
+-rw-r--r--   0 josh       (502) staff       (20)       38 2023-06-27 00:03:56.299970 contextplot-0.0.4/setup.cfg
+-rw-r--r--   0 josh       (502) staff       (20)      339 2023-06-27 00:03:38.000000 contextplot-0.0.4/setup.py
```

### Comparing `contextplot-0.0.3/LICENSE` & `contextplot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `contextplot-0.0.3/PKG-INFO` & `contextplot-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: contextplot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make Matplotlib plots in Jupyter notebooks using a context manager API
 Author: Josh Burkart
 Project-URL: Bug Tracker, https://gitlab.com/joshburkart/joshpyutil/-/issues
 Project-URL: Homepage, https://gitlab.com/joshburkart/joshpyutil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Make Matplotlib plots in Jupyter notebooks using a context manager API
 
-See [`example.ipynb`](https://gitlab.com/joshburkart/joshpyutil/-/blob/main/example.ipynb).
+See [`example.ipynb`](https://gitlab.com/joshburkart/contextplot/-/blob/main/example.ipynb).
```

### Comparing `contextplot-0.0.3/contextplot/__init__.py` & `contextplot-0.0.4/contextplot/__init__.py`

 * *Files identical despite different names*

### Comparing `contextplot-0.0.3/contextplot.egg-info/PKG-INFO` & `contextplot-0.0.4/contextplot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: contextplot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make Matplotlib plots in Jupyter notebooks using a context manager API
 Author: Josh Burkart
 Project-URL: Bug Tracker, https://gitlab.com/joshburkart/joshpyutil/-/issues
 Project-URL: Homepage, https://gitlab.com/joshburkart/joshpyutil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Make Matplotlib plots in Jupyter notebooks using a context manager API
 
-See [`example.ipynb`](https://gitlab.com/joshburkart/joshpyutil/-/blob/main/example.ipynb).
+See [`example.ipynb`](https://gitlab.com/joshburkart/contextplot/-/blob/main/example.ipynb).
```

### Comparing `contextplot-0.0.3/pyproject.toml` & `contextplot-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "Make Matplotlib plots in Jupyter notebooks using a context manager API"
 name = "contextplot"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.3"
+version = "0.0.4"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/joshburkart/joshpyutil/-/issues"
 "Homepage" = "https://gitlab.com/joshburkart/joshpyutil"
 
 [build-system]
 build-backend = "setuptools.build_meta"
```

