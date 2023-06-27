# Comparing `tmp/celery-batches-0.8.tar.gz` & `tmp/celery-batches-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-batches-0.8.tar", last modified: Tue Jun 27 14:30:30 2023, max compression
+gzip compressed data, was "celery-batches-0.8.1.tar", last modified: Tue Jun 27 17:03:05 2023, max compression
```

## Comparing `celery-batches-0.8.tar` & `celery-batches-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 14:30:30.788544 celery-batches-0.8/
--rw-r--r--   0 clokep     (501) staff       (20)     2770 2022-02-22 19:08:16.000000 celery-batches-0.8/LICENSE
--rw-r--r--   0 clokep     (501) staff       (20)     3549 2023-06-27 14:30:30.788704 celery-batches-0.8/PKG-INFO
--rw-r--r--   0 clokep     (501) staff       (20)     2052 2023-06-27 14:29:38.000000 celery-batches-0.8/README.rst
-drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 14:30:30.785794 celery-batches-0.8/celery_batches/
--rw-r--r--   0 clokep     (501) staff       (20)    11315 2022-10-24 19:42:02.000000 celery-batches-0.8/celery_batches/__init__.py
--rw-r--r--   0 clokep     (501) staff       (20)     2305 2022-04-08 19:20:36.000000 celery-batches-0.8/celery_batches/trace.py
-drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 14:30:30.788245 celery-batches-0.8/celery_batches.egg-info/
--rw-r--r--   0 clokep     (501) staff       (20)     3549 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/PKG-INFO
--rw-r--r--   0 clokep     (501) staff       (20)      283 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/SOURCES.txt
--rw-r--r--   0 clokep     (501) staff       (20)        1 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/dependency_links.txt
--rw-r--r--   0 clokep     (501) staff       (20)       17 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/requires.txt
--rw-r--r--   0 clokep     (501) staff       (20)       15 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/top_level.txt
--rw-r--r--   0 clokep     (501) staff       (20)      380 2022-04-08 19:20:36.000000 celery-batches-0.8/pyproject.toml
--rw-r--r--   0 clokep     (501) staff       (20)     1690 2023-06-27 14:30:30.789468 celery-batches-0.8/setup.cfg
+drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 17:03:05.505196 celery-batches-0.8.1/
+-rw-r--r--   0 clokep     (501) staff       (20)     2770 2022-02-22 19:08:16.000000 celery-batches-0.8.1/LICENSE
+-rw-r--r--   0 clokep     (501) staff       (20)     3551 2023-06-27 17:03:05.505320 celery-batches-0.8.1/PKG-INFO
+-rw-r--r--   0 clokep     (501) staff       (20)     2052 2023-06-27 14:29:38.000000 celery-batches-0.8.1/README.rst
+drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 17:03:05.503229 celery-batches-0.8.1/celery_batches/
+-rw-r--r--   0 clokep     (501) staff       (20)    11315 2022-10-24 19:42:02.000000 celery-batches-0.8.1/celery_batches/__init__.py
+-rw-r--r--   0 clokep     (501) staff       (20)     2305 2022-04-08 19:20:36.000000 celery-batches-0.8.1/celery_batches/trace.py
+drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 17:03:05.504970 celery-batches-0.8.1/celery_batches.egg-info/
+-rw-r--r--   0 clokep     (501) staff       (20)     3551 2023-06-27 17:03:05.000000 celery-batches-0.8.1/celery_batches.egg-info/PKG-INFO
+-rw-r--r--   0 clokep     (501) staff       (20)      283 2023-06-27 17:03:05.000000 celery-batches-0.8.1/celery_batches.egg-info/SOURCES.txt
+-rw-r--r--   0 clokep     (501) staff       (20)        1 2023-06-27 17:03:05.000000 celery-batches-0.8.1/celery_batches.egg-info/dependency_links.txt
+-rw-r--r--   0 clokep     (501) staff       (20)       17 2023-06-27 17:03:05.000000 celery-batches-0.8.1/celery_batches.egg-info/requires.txt
+-rw-r--r--   0 clokep     (501) staff       (20)       15 2023-06-27 17:03:05.000000 celery-batches-0.8.1/celery_batches.egg-info/top_level.txt
+-rw-r--r--   0 clokep     (501) staff       (20)      380 2022-04-08 19:20:36.000000 celery-batches-0.8.1/pyproject.toml
+-rw-r--r--   0 clokep     (501) staff       (20)     1693 2023-06-27 17:03:05.505897 celery-batches-0.8.1/setup.cfg
```

### Comparing `celery-batches-0.8/LICENSE` & `celery-batches-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-batches-0.8/PKG-INFO` & `celery-batches-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-batches
-Version: 0.8
+Version: 0.8.1
 Summary: Experimental task class that buffers messages and processes them as a list.
 Home-page: https://github.com/clokep/celery-batches
 Author: Patrick Cloke
 Author-email: clokep@patrick.cloke.us
 License: BSD
 Project-URL: Documentation, https://celery-batches.readthedocs.io
 Project-URL: Release notes, https://github.com/clokep/celery-batches/blob/main/CHANGELOG.rst
```

### Comparing `celery-batches-0.8/README.rst` & `celery-batches-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `celery-batches-0.8/celery_batches/__init__.py` & `celery-batches-0.8.1/celery_batches/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-batches-0.8/celery_batches/trace.py` & `celery-batches-0.8.1/celery_batches/trace.py`

 * *Files identical despite different names*

### Comparing `celery-batches-0.8/celery_batches.egg-info/PKG-INFO` & `celery-batches-0.8.1/celery_batches.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-batches
-Version: 0.8
+Version: 0.8.1
 Summary: Experimental task class that buffers messages and processes them as a list.
 Home-page: https://github.com/clokep/celery-batches
 Author: Patrick Cloke
 Author-email: clokep@patrick.cloke.us
 License: BSD
 Project-URL: Documentation, https://celery-batches.readthedocs.io
 Project-URL: Release notes, https://github.com/clokep/celery-batches/blob/main/CHANGELOG.rst
```

### Comparing `celery-batches-0.8/setup.cfg` & `celery-batches-0.8.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = celery-batches
-version = 0.8
+version = 0.8.1
 description = Experimental task class that buffers messages and processes them as a list.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Patrick Cloke
 author_email = clokep@patrick.cloke.us
 url = https://github.com/clokep/celery-batches
 keywords = task, job, queue, distributed, messaging, actor
 license = BSD
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: BSD License
 	Topic :: System :: Distributed Computing
 	Topic :: Software Development :: Object Brokering
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
@@ -31,15 +31,15 @@
 	Source = https://github.com/clokep/celery-batches
 	Funding = https://github.com/sponsors/clokep
 	Tracker = https://github.com/clokep/celery-batches/issues
 
 [options]
 packages = 
 	celery_batches
-install_requires = celery>=5.0,<5.3
+install_requires = celery>=5.0,<5.4
 python_requires = >=3.8
 
 [flake8]
 extend-ignore = E203
 max-line-length = 88
 
 [isort]
```

