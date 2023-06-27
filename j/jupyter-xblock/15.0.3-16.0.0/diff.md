# Comparing `tmp/jupyter-xblock-15.0.3.tar.gz` & `tmp/jupyter-xblock-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-xblock-15.0.3.tar", last modified: Mon May 22 05:17:46 2023, max compression
+gzip compressed data, was "jupyter-xblock-16.0.0.tar", last modified: Tue Jun 27 14:19:43 2023, max compression
```

## Comparing `jupyter-xblock-15.0.3.tar` & `jupyter-xblock-16.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:17:46.908167 jupyter-xblock-15.0.3/
--rw-rw-r--   0 regis     (1000) regis     (1000)    35139 2023-05-22 04:46:45.000000 jupyter-xblock-15.0.3/LICENSE.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       41 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.3/MANIFEST.in
--rw-rw-r--   0 regis     (1000) regis     (1000)     4574 2023-05-22 05:17:46.904167 jupyter-xblock-15.0.3/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     3874 2023-05-22 04:49:23.000000 jupyter-xblock-15.0.3/README.md
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:17:46.904167 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)     4574 2023-05-22 05:17:46.000000 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)      359 2023-05-22 05:17:46.000000 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-22 05:17:46.000000 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       58 2023-05-22 05:17:46.000000 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       21 2023-05-22 05:17:46.000000 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       14 2023-05-22 05:17:46.000000 jupyter-xblock-15.0.3/jupyter_xblock.egg-info/top_level.txt
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:17:46.904167 jupyter-xblock-15.0.3/jupyterxblock/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.3/jupyterxblock/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:17:46.904167 jupyter-xblock-15.0.3/jupyterxblock/static/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:17:46.904167 jupyter-xblock-15.0.3/jupyterxblock/static/css/
--rw-rw-r--   0 regis     (1000) regis     (1000)       95 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.3/jupyterxblock/static/css/student.css
--rw-rw-r--   0 regis     (1000) regis     (1000)     3878 2023-05-22 05:16:22.000000 jupyter-xblock-15.0.3/jupyterxblock/xblock.py
--rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-05-22 05:17:46.908167 jupyter-xblock-15.0.3/setup.cfg
--rwxrwxr-x   0 regis     (1000) regis     (1000)     1148 2023-05-22 05:17:37.000000 jupyter-xblock-15.0.3/setup.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-27 14:19:43.332394 jupyter-xblock-16.0.0/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    35139 2023-05-22 04:46:45.000000 jupyter-xblock-16.0.0/LICENSE.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       41 2023-05-22 04:46:44.000000 jupyter-xblock-16.0.0/MANIFEST.in
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4966 2023-06-27 14:19:43.332394 jupyter-xblock-16.0.0/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3874 2023-05-22 04:49:23.000000 jupyter-xblock-16.0.0/README.md
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-27 14:19:43.320395 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4966 2023-06-27 14:19:43.000000 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)      359 2023-06-27 14:19:43.000000 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/SOURCES.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-06-27 14:19:43.000000 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/dependency_links.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       58 2023-06-27 14:19:43.000000 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/entry_points.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       21 2023-06-27 14:19:43.000000 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/requires.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       14 2023-06-27 14:19:43.000000 jupyter-xblock-16.0.0/jupyter_xblock.egg-info/top_level.txt
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-27 14:19:43.320395 jupyter-xblock-16.0.0/jupyterxblock/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-22 04:46:44.000000 jupyter-xblock-16.0.0/jupyterxblock/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-27 14:19:43.320395 jupyter-xblock-16.0.0/jupyterxblock/static/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-27 14:19:43.320395 jupyter-xblock-16.0.0/jupyterxblock/static/css/
+-rw-rw-r--   0 regis     (1000) regis     (1000)       95 2023-05-22 04:46:44.000000 jupyter-xblock-16.0.0/jupyterxblock/static/css/student.css
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3878 2023-05-22 05:16:22.000000 jupyter-xblock-16.0.0/jupyterxblock/xblock.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-06-27 14:19:43.332394 jupyter-xblock-16.0.0/setup.cfg
+-rwxrwxr-x   0 regis     (1000) regis     (1000)     1547 2023-06-27 14:19:20.000000 jupyter-xblock-16.0.0/setup.py
```

### Comparing `jupyter-xblock-15.0.3/LICENSE.txt` & `jupyter-xblock-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter-xblock-15.0.3/PKG-INFO` & `jupyter-xblock-16.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: jupyter-xblock
-Version: 15.0.3
+Version: 16.0.0
 Summary: Jupyter XBlock for Open edX
 Home-page: UNKNOWN
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://github.com/overhangio/jupyter-xblock
 Project-URL: Code, https://github.com/overhangio/jupyter-xblock
 Project-URL: Issue tracker, https://github.com/overhangio/jupyter-xblock/issues
 Project-URL: Community, https://discuss.openedx.com
 Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Jupyter XBlock
 
 This is an [XBlock](https://edx.readthedocs.io/projects/xblock-tutorial/en/latest/overview/introduction.html) to integrate JupyterHub notebooks to your [Open edX](https://openedx.org) learning management system (LMS).
```

### Comparing `jupyter-xblock-15.0.3/README.md` & `jupyter-xblock-16.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-xblock-15.0.3/jupyter_xblock.egg-info/PKG-INFO` & `jupyter-xblock-16.0.0/jupyter_xblock.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: jupyter-xblock
-Version: 15.0.3
+Version: 16.0.0
 Summary: Jupyter XBlock for Open edX
 Home-page: UNKNOWN
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://github.com/overhangio/jupyter-xblock
 Project-URL: Code, https://github.com/overhangio/jupyter-xblock
 Project-URL: Issue tracker, https://github.com/overhangio/jupyter-xblock/issues
 Project-URL: Community, https://discuss.openedx.com
 Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Jupyter XBlock
 
 This is an [XBlock](https://edx.readthedocs.io/projects/xblock-tutorial/en/latest/overview/introduction.html) to integrate JupyterHub notebooks to your [Open edX](https://openedx.org) learning management system (LMS).
```

### Comparing `jupyter-xblock-15.0.3/jupyterxblock/xblock.py` & `jupyter-xblock-16.0.0/jupyterxblock/xblock.py`

 * *Files identical despite different names*

