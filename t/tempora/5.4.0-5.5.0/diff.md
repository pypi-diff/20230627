# Comparing `tmp/tempora-5.4.0.tar.gz` & `tmp/tempora-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempora-5.4.0.tar", last modified: Tue Jun 27 08:55:02 2023, max compression
+gzip compressed data, was "tempora-5.5.0.tar", last modified: Tue Jun 27 09:14:01 2023, max compression
```

## Comparing `tempora-5.4.0.tar` & `tempora-5.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.851325 tempora-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 08:54:43.000000 tempora-5.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 08:54:43.000000 tempora-5.4.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.843325 tempora-5.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 08:54:43.000000 tempora-5.4.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 08:54:43.000000 tempora-5.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.843325 tempora-5.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-27 08:54:43.000000 tempora-5.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-27 08:54:43.000000 tempora-5.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 08:54:43.000000 tempora-5.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-27 08:54:43.000000 tempora-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-27 08:54:43.000000 tempora-5.4.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-27 08:55:02.851325 tempora-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-27 08:54:43.000000 tempora-5.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 08:54:43.000000 tempora-5.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.843325 tempora-5.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-27 08:54:43.000000 tempora-5.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 08:54:43.000000 tempora-5.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-27 08:54:43.000000 tempora-5.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 08:54:43.000000 tempora-5.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 08:54:43.000000 tempora-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 08:54:43.000000 tempora-5.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-27 08:55:02.851325 tempora-5.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.847325 tempora-5.4.0/tempora/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/utc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.847325 tempora-5.4.0/tempora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.851325 tempora-5.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-27 08:54:43.000000 tempora-5.4.0/tests/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 08:54:43.000000 tempora-5.4.0/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 08:54:43.000000 tempora-5.4.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 08:54:43.000000 tempora-5.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.828022 tempora-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 09:13:38.000000 tempora-5.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 09:13:38.000000 tempora-5.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.824022 tempora-5.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:13:38.000000 tempora-5.5.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:13:38.000000 tempora-5.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.824022 tempora-5.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-27 09:13:38.000000 tempora-5.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-27 09:13:38.000000 tempora-5.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 09:13:38.000000 tempora-5.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-27 09:13:38.000000 tempora-5.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-27 09:13:38.000000 tempora-5.5.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-27 09:14:01.828022 tempora-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-27 09:13:38.000000 tempora-5.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 09:13:38.000000 tempora-5.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.824022 tempora-5.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-27 09:13:38.000000 tempora-5.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:13:38.000000 tempora-5.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-27 09:13:38.000000 tempora-5.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 09:13:38.000000 tempora-5.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 09:13:38.000000 tempora-5.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 09:13:38.000000 tempora-5.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-27 09:14:01.828022 tempora-5.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.824022 tempora-5.5.0/tempora/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-27 09:13:38.000000 tempora-5.5.0/tempora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-27 09:13:38.000000 tempora-5.5.0/tempora/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-27 09:13:38.000000 tempora-5.5.0/tempora/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-27 09:13:38.000000 tempora-5.5.0/tempora/utc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.828022 tempora-5.5.0/tempora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-27 09:14:01.000000 tempora-5.5.0/tempora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 09:14:01.000000 tempora-5.5.0/tempora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:14:01.000000 tempora-5.5.0/tempora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 09:14:01.000000 tempora-5.5.0/tempora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:14:01.000000 tempora-5.5.0/tempora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:14:01.000000 tempora-5.5.0/tempora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:14:01.828022 tempora-5.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-27 09:13:38.000000 tempora-5.5.0/tests/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 09:13:38.000000 tempora-5.5.0/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 09:13:38.000000 tempora-5.5.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 09:13:38.000000 tempora-5.5.0/tox.ini
```

### Comparing `tempora-5.4.0/.github/workflows/main.yml` & `tempora-5.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/LICENSE` & `tempora-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/NEWS.rst` & `tempora-5.5.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.5.0
+======
+
+Features
+--------
+
+- Stopwatch now uses ``time.monotonic``.
+
+
 v5.4.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `tempora-5.4.0/PKG-INFO` & `tempora-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.4.0
+Version: 5.5.0
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tempora-5.4.0/README.rst` & `tempora-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/docs/conf.py` & `tempora-5.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/docs/index.rst` & `tempora-5.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/pytest.ini` & `tempora-5.5.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/setup.cfg` & `tempora-5.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tempora/__init__.py` & `tempora-5.5.0/tempora/__init__.py`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tempora/schedule.py` & `tempora-5.5.0/tempora/schedule.py`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tempora/timing.py` & `tempora-5.5.0/tempora/timing.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,28 +44,29 @@
     def __init__(self):
         self.reset()
         self.start()
 
     def reset(self):
         self.elapsed = datetime.timedelta(0)
         with contextlib.suppress(AttributeError):
-            del self.start_time
+            del self._start
+
+    def _diff(self):
+        return datetime.timedelta(seconds=time.monotonic() - self._start)
 
     def start(self):
-        self.start_time = datetime.datetime.now(datetime.timezone.utc)
+        self._start = time.monotonic()
 
     def stop(self):
-        stop_time = datetime.datetime.now(datetime.timezone.utc)
-        self.elapsed += stop_time - self.start_time
-        del self.start_time
+        self.elapsed += self._diff()
+        del self._start
         return self.elapsed
 
     def split(self):
-        local_duration = datetime.datetime.now(datetime.timezone.utc) - self.start_time
-        return self.elapsed + local_duration
+        return self.elapsed + self._diff()
 
     # context manager support
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `tempora-5.4.0/tempora/utc.py` & `tempora-5.5.0/tempora/utc.py`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tempora.egg-info/PKG-INFO` & `tempora-5.5.0/tempora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.4.0
+Version: 5.5.0
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tempora-5.4.0/tempora.egg-info/SOURCES.txt` & `tempora-5.5.0/tempora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tests/test_schedule.py` & `tempora-5.5.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tests/test_timing.py` & `tempora-5.5.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `tempora-5.4.0/tox.ini` & `tempora-5.5.0/tox.ini`

 * *Files identical despite different names*

