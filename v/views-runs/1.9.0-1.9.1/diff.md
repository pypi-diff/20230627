# Comparing `tmp/views_runs-1.9.0.tar.gz` & `tmp/views_runs-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "views_runs-1.9.0.tar", max compression
+gzip compressed data, was "views_runs-1.9.1.tar", max compression
```

## Comparing `views_runs-1.9.0.tar` & `views_runs-1.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      415 2022-01-21 14:52:01.579709 views_runs-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1317 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/__init__.py
--rw-r--r--   0        0        0     4286 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/run.py
--rw-r--r--   0        0        0     1381 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/stats.py
--rw-r--r--   0        0        0     3816 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/storage.py
--rw-r--r--   0        0        0     4793 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/utilities.py
--rw-r--r--   0        0        0      666 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/validation.py
--rw-r--r--   0        0        0      111 2022-01-21 14:52:01.579709 views_runs-1.9.0/views_runs/vendoring.py
--rw-r--r--   0        0        0      677 2022-01-21 14:52:12.487822 views_runs-1.9.0/setup.py
--rw-r--r--   0        0        0      464 2022-01-21 14:52:12.488372 views_runs-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      422 2022-01-25 13:52:48.853006 views_runs-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1317 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/__init__.py
+-rw-r--r--   0        0        0     4286 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/run.py
+-rw-r--r--   0        0        0     1381 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/stats.py
+-rw-r--r--   0        0        0     3816 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/storage.py
+-rw-r--r--   0        0        0     4793 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/utilities.py
+-rw-r--r--   0        0        0      666 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/validation.py
+-rw-r--r--   0        0        0      111 2022-01-25 13:52:48.853006 views_runs-1.9.1/views_runs/vendoring.py
+-rw-r--r--   0        0        0      686 2022-01-25 13:53:00.173930 views_runs-1.9.1/setup.py
+-rw-r--r--   0        0        0      473 2022-01-25 13:53:00.174289 views_runs-1.9.1/PKG-INFO
```

### Comparing `views_runs-1.9.0/views_runs/__init__.py` & `views_runs-1.9.1/views_runs/__init__.py`

 * *Files identical despite different names*

### Comparing `views_runs-1.9.0/views_runs/run.py` & `views_runs-1.9.1/views_runs/run.py`

 * *Files identical despite different names*

### Comparing `views_runs-1.9.0/views_runs/stats.py` & `views_runs-1.9.1/views_runs/stats.py`

 * *Files identical despite different names*

### Comparing `views_runs-1.9.0/views_runs/storage.py` & `views_runs-1.9.1/views_runs/storage.py`

 * *Files identical despite different names*

### Comparing `views_runs-1.9.0/views_runs/utilities.py` & `views_runs-1.9.1/views_runs/utilities.py`

 * *Files identical despite different names*

### Comparing `views_runs-1.9.0/views_runs/validation.py` & `views_runs-1.9.1/views_runs/validation.py`

 * *Files identical despite different names*

### Comparing `views_runs-1.9.0/setup.py` & `views_runs-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['views_runs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['sklearn>=0.0,<0.1',
+['scikit-learn>=1.0.2,<2.0.0',
  'stepshift>=2.2.0,<2.3.0',
  'views-partitioning>=3.0.0,<4.0.0',
  'viewser>=5.7.3,<6.0.0']
 
 setup_kwargs = {
     'name': 'views-runs',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': '',
     'long_description': None,
     'author': 'peder2911',
     'author_email': 'pglandsverk@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

